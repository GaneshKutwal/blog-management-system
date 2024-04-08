1> Create a Virtual Environment
  - python -m venv env

2> Activate the Virtual Environment:
  - env\Scripts\activate  # For Windows
  - source env/bin/activate  # For Linux/Mac

3> Install Dependencies:
  - pip install -r requirements.txt
    
4>Start the Server:
  - python manage.py runserver

5> API Endpoints:
  - User Registration
      - Endpoint: http://127.0.0.1:8000/register/
      - Method: POST
      - Payload:
          {
              "username": "new_user1",
              "password": "new_password1"
          }
  - User Login:
      - Endpoint: http://127.0.0.1:8000/login/
      - Method: POST
      - Payload :
        {
            "username": "new_user1",
            "password": "new_password1"
        }
  - Create a Post
    
      - Endpoint: http://127.0.0.1:8000/posts/
      - Method: POST
      - Payload:
      {
          "title": "Sample Post Title",
          "content": "This is the content of the sample post."
      }

  - Get, Update, Delete a Post:
     - Endpoint: http://127.0.0.1:8000/posts/2/
     - Methods: GET, PUT, DELETE
     - Payload for Update (PUT):
     {
        "title": "Updated Post Title123",
        "content": "This is the updated content of the post."
    }

  - Comments on a Post:
      - Endpoint: http://127.0.0.1:8000/posts/2/comments/
      - Methods: GET, POST, PUT
      - Payload for Creating a Comment (POST):
      {
         "post": 2,
         "text": "This is a sample comment for the post."
      }

        


      



