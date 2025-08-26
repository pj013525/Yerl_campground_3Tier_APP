Yelp campground Application :-
==========================
This is a node.js application 
Tools used in this project are
--> Node js (npm)
--> Cloudinary
--> Mapbox
--> MangoDB


This is in Local, Dev and Prod level environments deployment.


Local Level Environment Deployment
----------------------------------------------------
Step1:- Set-up Server (t3.medium,ubuntu, volume:-28gb) and launch using any terminal agent.
======
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"
\. "$HOME/.nvm/nvm.sh"
nvm install 22
<img width="1356" height="705" alt="image" src="https://github.com/user-attachments/assets/97fcd527-e71a-48f6-ad16-2be3d6b12456" />


Step2:-    Now go to browser and search Cloudinary and create a free account in it
======
From API keys section, copy the cloud_name,  API_KEY,  API_SECRET

CLOUDINARY_CLOUD_NAME=dolehudbt
CLOUDINARY_KEY=169829682957635
CLOUDINARY_SECRET=jfwopyYy7EADVQnEm6MzPBBoZOQ
<img width="1366" height="680" alt="image" src="https://github.com/user-attachments/assets/cbafefa3-8e17-4ccd-9b2d-158f3c38f935" />


Step3:-   Now again in Browser search for Mapbox and create a free account in it
======
From Admin ==>Token ==> Copy the Default Token 

MAPBOX_TOKEN=pk.eyJ1IjoicGowMTM1MjUiLCJhIjoiY21lc2NpMTFnMDExazJtczlydXI5NTUxYSJ9.XO0W8sEeNQdY6cK9cdnF-Q
<img width="1364" height="681" alt="image" src="https://github.com/user-attachments/assets/2df1a42e-bac5-4869-bd3e-5268e1ab1389" />


Step4:-   Now search for Mongo atlas and sign up in it
======
Click on create cluster and give any name , provider and region near to you
Then copy the Username and Password that poped up

Username: rajjonna143
Password: EZlFoMmGtuCTNcOQ

CLick on create Database user ==> Drivers then copy the URL

DB_URL="mongodb+srv://rajjonna143:sWTLJYXzNTuhl1vV@pj.fculous.mongodb.net/?retryWrites=true&w=majority&appName=PJ"
SECRET=pj013525     #anything id fine here
<img width="1365" height="676" alt="image" src="https://github.com/user-attachments/assets/8643229e-d15f-4c7d-96c3-9d0b0f652062" />
<img width="1355" height="681" alt="image" src="https://github.com/user-attachments/assets/fc86b3f8-0587-4c7f-8691-22420ca722d6" />



Step5:-   Clone the git repo into the server and go into the server
======
git clone https://github.com/pj013525/Yerl_campground_3Tier_APP.git
cd Yerl_campground_3Tier_APP.git

npm install   # to install dependencies
vi .env ==> Paste

You can encode them using base64 also

CLOUDINARY_CLOUD_NAME=dolehudbt                                           #echo -n dolehudbt | base64
CLOUDINARY_KEY=169829682957635
CLOUDINARY_SECRET=jfwopyYy7EADVQnEm6MzPBBoZOQ
MAPBOX_TOKEN=pk.eyJ1IjoicGowMTM1MjUiLCJhIjoiY21lc2NpMTFnMDExazJtczlydXI5NTUxYSJ9.XO0W8sEeNQdY6cK9cdnF-Q
DB_URL="mongodb+srv://rajjonna143:sWTLJYXzNTuhl1vV@pj.fculous.mongodb.net/?retryWrites=true&w=majority&appName=PJ"
SECRET=pj013525  
	   
npm start       # To connect the Database successfully
<img width="1173" height="397" alt="image" src="https://github.com/user-attachments/assets/0904e6b3-7335-4821-9459-30c09f60d41c" />

Now check the Deployment in local environment using IP:3000
<img width="1365" height="674" alt="image" src="https://github.com/user-attachments/assets/b7f53764-ba1f-48b0-9d2f-ab4a459c4920" />


Step6:-     You can now register and Create, Read, Update, Delete your data and your data will be stored in Mongodb safely.
=======
<img width="1355" height="673" alt="image" src="https://github.com/user-attachments/assets/80c1349b-2f82-4cfd-90f6-55a98c6e0d80" />
<img width="1347" height="679" alt="image" src="https://github.com/user-attachments/assets/0f4c9f4e-5163-4a9c-b469-5fa225ddc7cd" />
<img width="1165" height="602" alt="image" src="https://github.com/user-attachments/assets/575cea63-6c56-4848-80d9-6650d4bd5e79" />

Step7:-   You can check your data in the Database also
=======
<img width="1366" height="634" alt="image" src="https://github.com/user-attachments/assets/93adb623-9ce8-427c-80be-1198c562aee8" />




