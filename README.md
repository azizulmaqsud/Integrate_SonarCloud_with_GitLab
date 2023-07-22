# Integrate and Start Sonar Cloud with GitLab

- Sign in to Sonar Cloud with Gitlab https://sonarcloud.io/welcome 
- Click on "Analyze your first projects" 
- Create Personal Access Tokens >> go back with duplicate broswer >> edit your profile >> Click on "Access Token" >> Token Name >> click on 'api' >> Create >> Copy & save in local
- Choose your analyze method >> Here I click on CICD Pipeline 
- Analyze a project with GitLab CI/CD Pipeline >> Follow the steps

# Steps 1

- Add environment variables

- a. Define the SonarCloud Token environment variable

    In GitLab, go to Settings > CI/CD > Variables to add the following variable and make sure it is available for your project:

        In the Key field, enter SONAR_TOKEN

	In the Value field, enter (see your page)

    Make sure that the Protect variable checkbox is unticked

    Make sure that the Mask variable checkbox is ticked

- b. Define the SonarCloud URL environment variable

 Still in Settings > CI/CD > Variables add a new variable and make sure it is available for your project:

    In the Key field, enter SONAR_HOST_URL

    In the Value field, enter https://sonarcloud.io

    Make sure that the Protect variable checkbox is unticked
    No need to tick the Mask variable checkbox this time

- Create or update a .gitlab-ci.yml file

What option best describes your build?

    Maven Gradle C,C++ or ObjC  Other (for JS, TS, Go, Python, PHP, ...)


# Step 2

- go to project CICD >> expand variables >> Add and update the variable with token
- go to code >> Repository >> recheck your .gitlab-ci.yml file
- go to build >> jobs 
- go to My Projects >> see the sonar scanning report !

# Success, Sonar Scanning Satrted !!

# Thank You!!

# Stay Connected !!

https://www.youtube.com/channel/UCNwP7KEElaJ7cdDTLP-KbBg

https://www.linkedin.com/in/azizul-maqsud/

https://azizulmaqsud-1684501031000.hashnode.dev/

https://medium.com/@azizulmaqsud

https://twitter.com/Sohail2me

https://github.com/azizulmaqsud
