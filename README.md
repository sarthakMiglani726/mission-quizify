# Mission Quizify

### Mission Scenario
In today's educational landscape, students and learners face challenges in reinforcing their understanding of various topics. Access to timely feedback and the ability to engage in unlimited practice are often limited. Recognizing this gap, our team has developed an AI-generated assessment and quiz tool. This tool provides users with instant feedback and comprehensive explanations, facilitating deeper comprehension and retention of knowledge. By dynamically generating quizzes based on user-provided documents, ranging from textbooks to scholarly papers, the tool offers a tailored learning experience. The end result is a user-friendly platform that empowers individuals to hone their skills, solidify their understanding, and ultimately excel in their academic pursuits.

### Features
- **Dynamic Quiz Generation**: Create quizzes based on user-uploaded documents.
- **Instant Feedback**: Receive immediate feedback on quiz answers with detailed explanations.
- **Customizable Quiz Topics**: Generate quizzes tailored to specific topics of interest.
- **User-Friendly Interface**: Easily navigate through quiz questions with a simple and intuitive interface.

### Getting Started

#### Prerequisites
1. **Google Cloud Account**: Set up a Google Cloud account for AI projects.
2. **Vertex AI APIs**: Enable Vertex AI APIs in your Google Cloud project.
3. **Service Account**: Create and manage service accounts with owner permissions.

#### Setting Up Google Cloud
1. **Create a Google Cloud Account**
2. **Set Up a Project**: Create a new project in the Google Cloud Console.
3. **Enable Vertex AI APIs**: Go to the APIs & Services dashboard and enable the Vertex AI APIs.
4. **Service Account Permissions**: Create a service account with owner permissions and download the key file.

#### Cloning the Repository
1. **Clone the Repository**: 
    ```bash
    git clone https://github.com/sarthakMiglani726/mission-quizify.git
    cd mission-quizify
    ```
    
2. **Create and activate a virtual environment**:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. **Install Dependencies**: 
    ```bash
    pip install -r requirements.txt
    ```

#### Configuration
1. **Service Account Key**: Place the downloaded service account key file in the project directory.
2. **Environment Variables**: Set up environment variables for authentication:
    ```bash
    export GOOGLE_APPLICATION_CREDENTIALS="path/to/your/service-account-key.json"
    ```

### Running the Application
1. **Start the Streamlit App**:
    ```bash
    streamlit run tasks/task_3/task_10.py
    ```

### Project Structure
- `tasks/task_3/task_10.py`: Main application file for the Streamlit interface.
- `tasks/task_3/task_3.py`: Document processing module.
- `tasks/task_4/task_4.py`: Embedding client module.
- `tasks/task_5/task_5.py`: Chroma collection creation module.
- `tasks/task_8/task_8.py`: Quiz generation module.
- `tasks/task_9/task_9.py`: Quiz management module.
- `requirements.txt`: Python dependencies.

### Usage
1. **Load Data**: Upload PDFs for ingestion and specify the quiz topic.
2. **Generate Quiz**: Configure the number of questions and generate the quiz.
3. **Take Quiz**: Answer the generated questions and receive instant feedback.

