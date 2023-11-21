# app
Practice application reading data from local json file and using react router and use in firebase
Task 	Associated APIs / Functions 	Description / Operation 
Initialization and Imports 	Import statements 	Import required modules 
 	useState, useEffect from 'react' 	Import React hooks 
 	db from './fbconfig' 	Import Firebase DB configuration 
 	Firestore and Storage functions 	Import Firestore and Storage APIs 
 	CRUD component 	Import the CRUD component 
State Variables 	useState for data fields and UI state 	Manage component state 
 	image for image file 	Handle selected image 
Upload Image 	ref, uploadBytesResumable from Storage API 	Upload image to Firebase Storage 
 	image state variable 	Select and upload an image 
Firestore Collection 	collection from Firestore API 	Reference to Firestore collection 
 	'scp-data' 	Name of Firestore collection 
Fetching Data (useEffect) 	useEffect 	Fetch data on component mount 
 	getDocs from Firestore API 	Retrieve documents from Firestore collection 
 	OurCollection reference 	Reference to 'scp-data' collection 
 	setReadData state variable 	Update state with retrieved data 
Create Document (CRUD) 	add Doc from Firestore API 	Add a new document to Firestore collection 
 	OurCollection reference 	Reference to 'scp-data' collection 
 	dataName, dataDescription, dataContainment 	Data entered for the new document 
Delete Document (CRUD) 	deleteDoc, doc from Firestore API 	Delete a document from Firestore collection 
 	OurCollection reference 	Reference to 'scp-data' collection 
 	id of the document to be deleted 	Unique document identifier 
Show/Edit Document (CRUD) 	showEdit function 	Display document for editing 
 	id, Name, Description, Containment 	Document details to edit 
 	setDataName, setDataDescription, setDataContainment, setId, setShowDoc 	Update UI state with document details 
Update Document (CRUD) 	updateDoc, doc from Firestore API 	Update an existing document in Firestore collection 
 	OurCollection reference 	Reference to 'scp-data' collection 
 	dataName, dataDescription, dataContainment 	New data entered for the document 
 	Reset form fields and UI state 	Clear form fields and exit editing mode 
Handle Image Change 	handleImageChange function 	Update 'image' state variable with selected image 
 	e.target.files[0] 	Selected image file 
Render JSX 	JSX for input fields, buttons, and document list 	Display UI components 
 	Loop through 'readData' and display documents 	Display document list 
 	Buttons for Create, Update, Delete operations 	Perform CRUD operations 
