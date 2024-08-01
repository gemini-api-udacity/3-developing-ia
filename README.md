# 3 Developing with Gemini API

1. [Introduction](#schema1)

[DOC](#schemadoc)


<hr>
<a name='schema1'></a>


## 1. Introduction

### Application Programming Interfaces (APIs)
Remember, an application programming interface (API) allows computer programs to communicate using a predetermined protocol. We are going to use the Gemini API so our Python code can communicate with the Gemini family of large language models!

![API](./img/api.jpg)

### Gemini API Keys
#### Introduction

We interact with APIs using API keys. A key is a unique identifier that is passed along with API requests to authenticate the client making the request. It helps ensure that only authorized users or applications can access the API and its services.

Note that for the Gemini API, there are two ways of creating a key:

#### Personal use
As part of an organization. Note: You need to ask your admin owner to grant you access to the "Early Access Apps" setting!
Between these two methods, the rest of the setup is the same.

**Important:** After generating these keys, keep them secure, you should never post them public or give them out. Treat them like passwords!

#### Creating a Gemini API Key
1. Navigate to the Google AI for Developers [home page](ai.google.dev)
2. Scroll down and click on the button "Get API Key in Google AI Studio"
3. Click "Create API Key" and "Create API key in new project" if you have not made a project before
4. Copy the key

### Google Colaboratory (Colab)
#### Introduction
Google Colaboratory, or Colab for short, is a free Jupyter Notebook service from Google. We will use Colab notebooks for our Python code in the rest of this course.

You can create a new Colab notebook by navigating to https://colab.new/. To follow along with the course content, click the "Open in Colab" buttons.

Google Colab shows a warning when you open a notebook that was not authored by Google. Click "Run anyway" when you see the message about the notebook being loaded from GitHub.

### Adding Your API Key to Google Colab
1. Open a Colab notebook
2. Click on the Secrets tab on the left side menu (represented by a key icon)
3. Click "Add new secret", type GOOGLE_API_KEY in the "Name" field, and paste your key in the "Value" field
4. Toggle the "Notebook access" switch to be "on" (represented by a checkmark)


**Important:** 
Use Jupyter Notebook:

You have the option to download the notebooks from the repository linked above and to use a local Jupyter Notebook environment, but you will need to adjust some of the code. For example, instead of using `from google.colab import userdata and GOOGLE_API_KEY = userdata.get("GOOGLE_API_KEY")`, you might use `import os and GOOGLE_API_KEY = os.environ["GOOGLE_API_KEY"]`. We will only be providing the Colab version of the code in this course.


[DOC](#schemadoc)
- [Excercise and Demo, Udacity](https://github.com/udacity/gemini-api-course)