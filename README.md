[![Resume Matcher](Assets/img/header.png)](https://www.resumematcher.fyi)

<div align="center">

# Resume Matcher

### AI Based Free & Open Source ATS, Resume Matcher to tailor your resume to a job description. Find the best keywords, and gain deep insights into your resume.

</div>

<br>

<div align="center">

![Stars](https://img.shields.io/github/stars/srbhr/Resume-Matcher?style=flat-square&color=EA1179)
![Apache 2.0](https://img.shields.io/github/license/srbhr/Resume-Matcher?style=flat-square&color=525FE1) ![Issues](https://img.shields.io/github/issues/srbhr/Resume-Matcher?style=flat-square&color=F86F03) ![Forks](https://img.shields.io/github/forks/srbhr/Resume-Matcher?style=flat-square&color=0079FF) [![Powered by Qdrant](https://img.shields.io/badge/Vector_search_by-Qdrant-982176?style=flat-square)](https://github.com/qdrant/qdrant)

[![Discord](https://custom-icon-badges.demolab.com/badge/Join%20Discord-blue?style=flat-square&logo=discord&color=F0FF42&logoColor=293462)](https://discord.gg/t3Y9HEuV34)
[![Resume Matcher](https://custom-icon-badges.demolab.com/badge/www.resumematcher.fyi-gold?style=flat-square&logo=globe&logoColor=black)](https://www.resumematcher.fyi)
[![Resume Matcher](https://custom-icon-badges.demolab.com/badge/Live_Demo_on_Streamlit-green?style=flat-square&logo=live&color=F55353)](https://resume-matcher.streamlit.app/)

<a href="https://www.producthunt.com/posts/resume-matcher?utm_source=badge-featured&utm_medium=badge&utm_souce=badge-resume&#0045;matcher" target="_blank"><img src="https://api.producthunt.com/widgets/embed-image/v1/featured.svg?post_id=401261&theme=light" alt="Resume&#0032;Matcher - Free&#0032;and&#0032;Open&#0045;Source&#0032;ATS&#0032;Tool&#0032;to&#0032;Match&#0032;Resumes&#0032;to&#0032;Job&#0032;Desc&#0046; | Product Hunt" style="width: 180px; height: 50px;" width="200" height="54"/></a>

</div>

<div align="center">

## How does it work?

</div>

The Resume Matcher takes your resume and job descriptions as input, parses them using Python, and mimics the functionalities of an ATS, providing you with insights and suggestions to make your resume ATS-friendly.

The process is as follows:

1. **Parsing**: The system uses Python to parse both your resume and the provided job description, just like an ATS would. Parsing is critical as it transforms your documents into a format the system can readily analyze.

2. **Keyword Extraction**: The tool uses advanced machine learning algorithms to extract the most relevant keywords from the job description. These keywords represent the skills, qualifications, and experiences the employer seeks.

3. **Key Terms Extraction**: Beyond keyword extraction, the tool uses textacy to identify the main key terms or themes in the job description. This step helps in understanding the broader context of what the resume is about.

4. **Vector Similarity Using Qdrant**: The tool uses [Qdrant](https://github.com/qdrant/qdrant), a highly efficient vector similarity search tool, to measure how closely your resume matches the job description. This process is done by representing your resume and job description as vectors in a high-dimensional space and calculating their cosine similarity. The more similar they are, the higher the likelihood that your resume will pass the ATS screening.

On top of that, there are various data visualizations that I've added to help you get started.

<div align="center">

## How to install

</div>

Follow these steps to set up the environment and run the application.

1. Fork the repository [here](https://github.com/srbhr/Resume-Matcher).

2. Clone the forked repository.

    ```bash
    git clone https://github.com/<YOUR-USERNAME>/Resume-Matcher.git
    cd Resume-Matcher
    ```

3. Create a Python Virtual Environment:

    - Using [virtualenv](https://learnpython.com/blog/how-to-use-virtualenv-python/):

        _Note_: Check how to install virtualenv on your system here [link](https://learnpython.com/blog/how-to-use-virtualenv-python/).

        ```bash
        virtualenv env
        ```

    **OR**

    - Create a Python Virtual Environment:

        ```bash
        python -m venv env
        ```

4. Activate the Virtual Environment.

    - On Windows.

        ```bash
        env\Scripts\activate
        ```

    - On macOS and Linux.

        ```bash
        source env/bin/activate
        ```

5. Install Dependencies:

    ```bash
    pip install -r requirements.txt
    ```

6. Prepare Data:

    - Resumes: Place your resumes in PDF format in the `Data/Resumes` folder. Remove any existing contents in this folder.
    - Job Descriptions: Place your job descriptions in PDF format in the `Data/JobDescription` folder. Remove any existing contents in this folder.

7. Parse Resumes to JSON:

    ```python
    python run_first.py
    ```

8. Run the Application:

    ```python
    streamlit run streamlit_app.py
    ```

**Note**: For local versions, you do not need to run "streamlit_second.py" as it is specifically for deploying to Streamlit servers.

**Additional Note**: The Vector Similarity part is precomputed to optimize performance due to the resource-intensive nature of sentence encoders that require significant GPU and RAM resources. If you are interested in leveraging this feature in a Google Colab environment for free, refer to the upcoming blog (link to be provided) for further guidance.

<br/>

### Docker

1. Build the image and start application

    ```bash
        docker-compose up
    ```

2. Open `localhost:80` on your browser

<br/>

<div align="center">

## Join Us, Contribute! 💡

</div>

Pull Requests & Issues are not just welcomed, they're celebrated! Let's create together.

🎉 Join our lively [Discord](https://dsc.gg/resume-matcher) community and discuss away!

💡 Spot a problem? Create an issue!

👩‍💻 Dive in and help resolve existing [issues](https://github.com/srbhr/Resume-Matcher/issues).

🔔 Share your thoughts in our [Discussions & Announcements](https://github.com/srbhr/Resume-Matcher/discussions).

🚀 Explore and improve our [Landing Page](https://github.com/srbhr/website-for-resume-matcher). PRs always welcome!

#### Tech Stack

Current:

![](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&color=blue&logoColor=green)

Upcoming:

![](https://img.shields.io/badge/Python-14354C?style=flat-square&logo=python&logoColor=white) ![](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white) ![](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![](https://custom-icon-badges.demolab.com/badge/Fast_API-F11A7B?style=flat-square&logo=python&logoColor=22A699)

<br/>

<div align="center">

## Enhance Open-Source Development: Donate and Be Part of Our Journey!

[![BuyMeACoffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://buymeacoffee.com/srbhr)
[![Sponsor on GitHub](https://img.shields.io/badge/sponsor-30363D?style=for-the-badge&logo=GitHub-Sponsors&logoColor=#white)](https://github.com/sponsors/srbhr)

</div>

---

### Heads Up! 📝

Your support means the world to us 💙. We're nurturing this project with an open-source community spirit, and we have an ambitious roadmap ahead! Here are some ways you could contribute and make a significant impact:

✨ Transform our Streamlit dashboard into something more robust.

📚 Enhance our functionality by enabling resume upload and parsing.

🐳 Simplify usage by adding a Docker image.

💡 Improve our parsing algorithm, making data more accessible.

🖋 Share your insights and experiences in a blog post to help others.

🎨 Give our [landing page](https://github.com/srbhr/website-for-resume-matcher) a fresh look using React, Vue, or your preferred framework.

Take the leap, contribute, and let's grow together! 🚀

---

### Our Contributors ✨

<a href="https://github.com/srbhr/Resume-Matcher/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=srbhr/Resume-Matcher" />
</a>
