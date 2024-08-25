<div align="center">
<a href="https://summerofcode.withgoogle.com/projects/#6521788818784256"><img src="https://i.imgur.com/pgkUceb.png" width="650" alt="google-summer-of-code"></a>
<br>
</div>

<br>
<br>

<p align="center">
<code> <a href="#-project-overview">Project Overview</a>&nbsp;&nbsp;&nbsp; <a href="#-deliverables">Deliverables</a>&nbsp;&nbsp;&nbsp; <a href="#-demo">Demo</a>&nbsp;&nbsp;&nbsp; <a href="#-contributions">Contributions</a>&nbsp;&nbsp;&nbsp; <a href="#-mentors">Mentors</a>&nbsp;&nbsp;&nbsp; <a href="#-links">Links</a>
</code>
</p>

<br>
<br>

## ⭐ Project Overview
The `Google Summer of Code Community Hub` project for Rocket.Chat represents a significant leap forward in fostering open-source collaboration and community engagement.
At its core, the project focused on two pivotal areas:

`Syntax Sweetening:` This involved developing an innovative approach to server-side customization and configurability. By introducing HTML-tag-like notation into component layout files, we simplified the process of creating and maintaining community portals. This enhancement allows for easier generation of layouts through WYSIWYG (What You See Is What You Get) IDE tools, making the platform more accessible to developers of all skill levels.

`Component Initialization Data Definition and Maintenance:` We tackled the complex challenge of managing component data, creating a robust system that streamlines how data is defined, initialized, and maintained across the platform. This solution enhances the flexibility and scalability of the Community Hub, allowing it to adapt to the diverse needs of various open-source communities.

The project's overarching goal was to create a more intuitive, customizable, and efficient platform that serves as a central hub for open-source organizations participating in Google Summer of Code. By leveraging advanced technologies and methodologies, we aimed to:

- Simplify the development process for community builders
-  Enhance collaboration and communication among open-source teams
- Provide a scalable solution that can grow with communities of all sizes
- Offer a highly customizable platform that can be tailored to each organization's unique needs
- Improve the overall user experience for both developers and community members

This year's work extends the capabilities to create a more powerful and user-friendly environment. The enhancements implemented during this GSoC project not only improve the current functionality but also pave the way for future innovations in open-source community management and collaboration.


## 📦 Deliverables
### 1. Syntax Sweetening Framework

- Developed a new syntax allowing web app creators to define component-based static sites in a single source file
- Implemented parsing of .agml files to generate React functional components

### 2. Build Pipeline Enhancement

- Modified the existing build process to accommodate customizations from syntax sweetened declaration files
- Implemented efficient integration of customizations at appropriate build stages

### 3. Component Creator Tooling

- Created a system to abstract away complexities of data handling for component creators
- Implemented functionality for component creators to define data directly in syntax sweetened declaration files
- Developed tooling to simplify the integration of dynamic data into static sites

### 4. Customization and Flexibility Improvements

- Enhanced the ability for open-source organizations to create unique and personalized community portals
Implemented features to allow easy modification of layout, colors, and components to match brand aesthetics and functional requirements


## 📺 Demo 
### 1. Syntax Sweetening Framework

### 2. Component Creator Tooling

### 3. Customization and Flexibility


### Upcoming Feature:

## 🚀 Contributions

## 🦾 Overcoming Challenges and breaking limits

### 1. Payload CMS vs. Strapi: Opting for Seamless Integration

- We chose `Payload CMS` over Strapi due to its code-first approach and seamless integration with Next.js. Unlike Strapi, which required running in a separate Docker container, Payload CMS allowed us to run everything within our existing Next.js environment.
- Payload CMS also stood out for its active and helpful community, which played a crucial role during the initial stages. I interacted directly with the core maintainers to implement Payload CMS 3.0 alpha, customizing it to our specific needs with build-time scripts. This hands-on collaboration enabled us to modulate the CMS effectively, setting a solid foundation for our project.

### 2. OAuth: Simplifying Authentication

- Initially, we considered implementing traditional OAuth, but after a deeper analysis, I realized that this approach would require running a separate authorization proxy server, which was unnecessary for our static site. 
- To explore this further, I built a prototype of OAuth that required a server. This experiment led to an in-depth discussion on the practicality of OAuth for our use case. Ultimately, we concluded that OAuth was an over-engineered solution for our needs, allowing us to pivot towards a simpler authentication solution using `FaunaDB`.

### 3. Project Structure: Streamlining for Simplicity

- The project underwent significant restructuring. Initially, we used a TurboRepo setup, but after multiple iterations, we simplified it. The final structure included a `build folder` for the Next.js static site and a `src folder` for .agml files and associated data. This streamlined structure made the project more manageable and efficient for the community builder.

### 4. Syntax Parsing: Transitioning from Regex to AST

- Our initial attempt at syntax sweetening using Ripgrep, a Rust-based grep tool and regex proved unreliable. After reconsidering, we switched to `Abstract Syntax Trees (AST)` for parsing .agml. I invested time in learning AST manipulation, eventually adopting the `TypeScript Compiler API`. This allowed us to effectively convert .agml into static Next.js web pages with better accuracy and flexibility.

- Fun fact: AGML stands for `Anjaneya Gupta Markup Language`—a name suggested by my mentor, Sing Li, and named after myself ;)

### 5. Dynamic Data Fetching: Balancing JSON and CMS Data

- Creating a dynamic data-fetching solution that worked with both JSON and CMS data presented challenges. We pondered over multiple approaches to ensure consistency between the two data sources and explored different methods, such as checking build numbers or using a flag during build-time. Prototyping various solutions helped us refine our approach and ensure consistency between data sources, leading to a more reliable and flexible system.

### 5. Bootstrap vs. Tailwind: Choosing a Flexible Front-End Framework

- In our front-end development, Bootstrap proved superior to Tailwind for our use case. Bootstrap offers responsive, pre-built components and allows easy CSS overrides through its syntax, reducing code complexity and streamlining development. This efficiency and simplicity made it ideal for our project. I created a `Proof of Concept (POC)` to demonstrate Bootstrap's advantages, which ultimately solidified our decision.

By prototyping early and iterating quickly, I was able to provide clear demonstrations that informed our decisions, making our development process more efficient and focused.

</div>

## ❤️ Support
Learned something new today? Reciprocate the love and ⭐ this repo for good karma.
    
## 🙌🏼 Mentors
I extend my sincere gratitude to my mentors for their invaluable guidance and support throughout this journey. Their expertise and encouragement were instrumental in overcoming challenges and pushing the boundaries of what we could achieve 🙏 

- **Sing Li** - [GitHub](https://github.com/](https://github.com/Sing-Li)). [LinkedIn](https://www.linkedin.com/in/sing-li-119716139/)

- **Palanikannan M** - [GitHub](https://github.com/). [LinkedIn](https://www.linkedin.com/in/)
  
## 👤 About Me
I'm a Computer Science student passionate about full-stack development, open-source contribution, and deep learning. What sets me apart is my strong problem-solving skills and my knack for finding creative solutions to complex challenges. I'9m a curious and inquisitive individual, always pushing the boundaries of what's possible and eager to collaborate on impactful projects.

## 🛤️ My Journey

My journey as a software engineer began with an insatiable fascination for technology and a burning desire to be at the forefront of innovation. During this journey, I have really upgraded my skills in frameworks such as Next.js whilst learning and applying languages such as Typescript, shell scripting, GoLang, SQL( Prisma + Zod). I’ve worked a lot on my DevOps skills as well while working at Zscaler as a DevOps Intern and building a MVP of a project ( Zcoder ~ an internal tool to generate unit test cases, provide code suggestions etc using the LLM trained on our private codebase)  which was presented to the board of the company!

## 💬 Connect With Me
<div align="center">

| **Student** | Nabhag Motivaras |
|:--------------------|:-------------------|
| **Organization** | [Rocket.Chat](https://rocket.chat/) |
| **Project** | []() |
| **GitHub** | [@anjy7](https://github.com/anjy7) |
| **LinkedIn** | [Anjaneya Gupta](https://www.linkedin.com/in/anjaneya-gupta/) |
| **Email** | <a href="mailto:anjyofficial@gmail.com">anjyofficial@gmail.com</a> |
| **Rocket.Chat** | [anjaneya.gupta](https://open.rocket.chat/direct/anjaneya.gupta) |
| **Project Github Repository** | []() |
       
</div>

