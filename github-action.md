* Workflow
* Events
* Jobs
* Steps
* Runners
  
# Sample Work flow Explanation ::
# first-workflow.yml 
# Every work flow has three mandatory things 
name: First Workflow # name of the workflow -shows in github UI
on: # when to run it - trigger /event
  workflow_dispatch: # runs when manually triggered 
jobs: # what to do 
  first-job:
    runs-on: ubuntu-latest # runners
    steps:
      - name : Print Welcome Message 
        run: echo "first workflow created by anki"
