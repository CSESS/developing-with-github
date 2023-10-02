# Developing with GitHub
This repository contains the resources and tasks for the seminar "Developing with GitHub". The seminar introduces GitHub's issue tracking and collaborative development features, including issues, pull requests, and actions. Here, we will try to fork the `CSESS/developing-with-github.git` repository, add an additional page to the fork, then submit a pull request based on the change.

## Seminar Details
Date: 3rd October, 2023  
Time: 18:30–19:30  
Venue: Lecture Theatre D, Academic Building, Hong Kong University of Science and Technology  
Host: [@usertam](https://github.com/usertam)

## Getting Started
To get started with the tasks, follow these steps:
1. Fork this repository to your own GitHub account. Click "Fork", then "Create Fork". The same repository should now be under your GitHub name.

2. Clone the repository to your local machine using the following command:
```
git clone https://github.com/<your_username>/developing-with-github.git
```

3. Create a new branch `feature/add-page` based on the default branch:
```
cd developing-with-github
git checkout -b feature/add-page
```

4. Open a new markdown file (.md) with your username, inside the directory `src/pages`. Write some feedback for [Samuel](https://github.com/usertam), praise [Desmond](https://www.cse.ust.hk/~desmond), or write something else really nice.
~~~
cat <<'EOF' > src/pages/<your_username>.md
# Letter to the Samuel on the Podium
```
From: Samuel Tam <hytamap@ust.hk>
To: Samuel Tam <hytamap@ust.hk>
Subject: Ganbatte on the "Developing with GitHub" Seminar!!!
Date: Mon, 2 Oct 2023 23:59:59 +0800
```

Dear Future Samuel on the Podium,

Doing this seminar and everything live must be really stressful.
But I do hope both the audience and you can take home something. :)

Best,
Samuel
EOF
~~~

5. Add the new file, commit the change, push to your forked repository.
```
git add src/pages
git commit -m "<your_username>: add page"
git status # sanity check
git log # more sanity check
git push origin feature/add-page
```

6. Visit your forked repository on GitHub (e.g., `https://github.com/<your-username>/developing-with-github`) and you should see a prompt to create a pull request for your branch. Click on the "Compare & pull request" button.

7. Review the changes you made and provide a clear description of the changes in the pull request. If necessary, add comments or additional information.

8. Satisfied with the pull request? Click on the "Create pull request" button to submit it.

9. Once your submitted pull request is accepted, you should see your markdown content rendered under `https://csess.github.io/developing-with-github/<your_username>`. For COMP4900 students, please submit your own **pull request link** (e.g., `https://github.com/CSESS/developing-with-github/pull/1`) to Canvas.

## Contributing
Contributions to this repository are not expected as it is primarily meant for the seminar attendees. However, if you have any suggestions or improvements, please feel free to open an issue in the repository.

## License
The project was bootstrapped with `yarn create astro`. The contents under `src/pages` of this repository are licensed under the MIT License.
