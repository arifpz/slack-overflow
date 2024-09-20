# Instructions
Welcome to the workshop! This is a hands-on workshop where you will learn how to build a Slack bot using Python. The bot will be able to search for questions on StackOverflow and return the top results to you.

Credit to [Karan Goel](https://github.com/karan/slack-overflow) for the original code.

## What will we learn
The main goal of this workshop to get sense how to deal with legacy code. I've put some isses on [issues page](https://github.com/arifpz/slack-overflow/issues), and we will try to fix them. Anyone can pick any issue and try to fix it. I will be here to help you with any questions you have.

- Prerequisites materials available here: [deck](https://link.excalidraw.com/p/readonly/7jlH8ujOxDwHYML0ZaOk)
- Fork the repo to contribute, then follow the instructions below to get the code running on your local machine.

## Make the code running
We aren't try to integrate it to slack (as the ideal origin flow), but if you want, you can follow this [steps](https://github.com/arifpz/slack-overflow?tab=readme-ov-file#integrate-with-your-team). We will do integration test locally using postman or curl.

### StackExchange credentials
Add a `config.py` file based on `config.py.example` file. Grab your StackExchange key from http://stackapps.com/

### Run the code
- Make sure you have python installed on your local machine, if not, follow this [steps](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/)
- If you haven't have git installed, you can follow this [steps](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- Fork the repo (can use UI)
- Clone the forked repo to your local machine
- Run the app
```python
# Install python dependencies
$ pip install -r requirements.txt

# Start the server
$ python app.py
```

- Here curl to test:
```bash
curl --location 'http://127.0.0.1:5000/overflow' \
--form 'text="postgres performance"'
```

## Having fun
- Pick your probelm you are interested in from [issues page](https://github.com/arifpz/slack-overflow/issues)
- Create a branch with the issue number as the branch name
- Fix the issue
- Push the branch to your fork
- Create a pull request
- Let's present: 
  - Explain your idea
  - Let's discuss the code

## References
- [Post about test in legacy code by Gergely Orosz](https://www.linkedin.com/posts/gergelyorosz_i-have-a-couple-of-side-projects-running-activity-7202283830219554817-yekz?utm_source=share&utm_medium=member_desktop)
- [A simpler way to understand legacy code](https://sourcegraph.com/blog/a-simpler-way-to-understand-legacy-code)
- Book: [**Working Effectively with Legacy Code by** Michael Feathers](https://prod-files-secure.s3.us-west-2.amazonaws.com/59b938ec-e05c-4dc1-a8c5-ef98243420ad/32709680-a227-4d4c-99ab-a9a26ee54700/Screenshot_2024-09-19_at_19.14.32.png)
    - Podcast: https://www.youtube.com/watch?v=P_6eDL1aqtA
    - Summary: https://gist.github.com/jonnyjava/42883d4e464167f81e2ee60a488a5ded
