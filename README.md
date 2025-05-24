##Prerequisites

-Python 3.12
- Git
- Jenkins (with plugins):
- Pipeline
- GitHub Integration
- Blue Ocean
- Email Extension Plugin
- Email configuration in Jenkins (SMTP setup and configure with Gmail)
- GitHub repository forked from:


##Install Dependencies
- Install and configured Jenkins on Local Ubuntu system
- Install Python and `pip` on Jenkins server
- Ensure Jenkins has access to the Python environment


##Clone Repo
- Found random flask project on githup fork and clone the same

##Jenkins Job
- Created a Jenkins pipeline
- Stages are devided with by tasks
- Enabled the trigger
- GitHub hook trigger for GITScm polling


##Jenkins Pipeline stages overview

### Build
- Creates a virtual environment
- Installs dependencies via pip

###Test
- Runs unit tests using pytest

###Deploy
- Starts Flask app with:
 --- bash
  flask --app flaskr run --host=0.0.0.0 --port=5000
