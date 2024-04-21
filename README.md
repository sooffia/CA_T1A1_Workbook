# CA_T1A1_Workbook
## by Sofia 
## Q1: **Identify** and **explain** common and important components and concepts of web development

Markup languages are crucial in web development as they define content structure, layout, and website presentation. Web developers must grasp markup languages to develop visually appealing, beneficial, and accessible websites that effectively communicate content. Developers can structure content (such as font size, colour, and style) and arrange it inside pages using these languages, which describe document layout and style through annotations like tags or elements. Examples are content structures specified with explicit tags using descriptive syntax, like in HTML and XML. Semantic markup, such as HTML components (lists, tables, and paragraphs) and header tags (H1, H2, and H3), helps search engines comprehend the context and hierarchy of material, which enhances indexing and visibility in search results (Ranked, n.d). 

## Q2: **Define** the features of the following technologies that are essential in terms of the development of the internet: 

> ### **Explain**  how each technology has contributed to the development of the internet.

### Packets:
Packet's primary features for the growth of the internet are their capacity to improve the scalability, dependability, and efficiency of data transfer. The little units in which data is divided and sent over the internet are called "packets." Packet segmentation, which separates data into smaller pieces, is one essential component. This segmentation enables more efficient transmission since smaller packets are less likely to be missed or distorted during transfer. More efficient transmission is made possible by this segmentation, as smaller packets have a lower probability of being lost or distorted in transit. Retransmitting a single packet, as opposed to the complete data stream, is necessary if they become lost or corrupted. This lessens the effect of network failures and guarantees dependable data delivery. The ability of individual packets to be routed independently along different network channels, maximising traffic flow and reducing congestion, is another essential component of packet routing flexibility. Multiple users can access and download content simultaneously without experiencing delays or bottlenecks due to its dynamic routing capabilities, which improve speed and responsiveness (MDN,2023). 

### IP Addresses (IPv4 and IPv6): 
The Internet functions as a worldwide network of computers, with each computer requiring a unique address for connectivity. The format of these addresses, also called IP (Internet Protocol) addresses, is nnn.nnn.nnn.nnn, with each nnn ranging from 0 to 255. This guarantees unique identification and efficient communication between devices that are connected. The figure shows two computers linked to the Internet: one has IP address 1.2.3.4, and the other has IP address 5.6.7.8. The Internet is an abstract object that makes these connections possible (Shuler, 2002). 

![figure screenshot](./assets/figure-1.png) 

Figure 1: How two computers connect (Shuler, 2002). 

An Internet Service Provider (ISP) usually assigns you a temporary IP address for the duration of your session when you connect to the internet. Your computer might acquire a temporary IP address from a DHCP (Dynamic Host Configuration Protocol) server or have a permanent one on a local area network (LAN). While linked to the internet, your computer always retains a distinct IP address. Comprehending the importance of IP addresses requires an examination of the two main varieties, IPv4 and IPv6, both of which are significant for enabling worldwide communication and meeting the increasing demand for unique identifiers in the digital domain (Shuler, 2002). The transition from IPv4 to IPv6 has significantly impacted how the internet has evolved. Due to limitations, IPv4, which was first introduced in 1983 and used a 32-bit address structure that could support 4.3 billion distinct addresses, was replaced in 1999 with IPv6. With the introduction of the 128-bit address format in IPv6, the number of addresses available to accommodate the increasing number of devices connected to the internet has dramatically increased. IPv6 also provides more room for addresses, adds better security with organized coding, makes routing simpler by cutting out extra steps, improves how addresses are set up and is ready for the internet to keep growing and improving. These are important for making the internet work smoothly (Hosting,n.d.). 

### Routers and Routing:
How do packets travel through the internet, and do all Internet-connected computers know where all the other computers are? The response to such questions is "no." Rather, the information required to direct packets to their destinations is contained in routing tables kept up to date by every router connected to the internet. In short, routers are traffic controllers for information on the internet. They act as a bridge across several networks, assisting by appropriately directing data packets. Although every router knows its networks and addresses, it may not know the broader picture beyond them. A central point connects more extensive NSP backbones at the top of Figure 2, and the black boxes in the diagram stand in for routers linking the significant networks. Smaller networks are located beneath these, while local networks with connected computers are at the bottom. This configuration facilitates effective data flow management across the internet (Shuler, 2002). 

![figure screenshot](./assets/figure-two.png) <br>
Figure 2: Networks for routers (Shuler, 2002). 

A router first examines the IP address of the sender computer's IP protocol layer appended to the packet. A router first examines the IP address of the sender computer's IP protocol layer appended to the packet. The packet is then directed to the network that matches the IP address if the router discovers it by consulting its routing database. By default, the router forwards the packet to the next router on the backbone hierarchy if the network cannot be located. This process is repeated until a router with the required data is reached. Large routing tables on routers linked to major backbones allow them to direct a packet to the appropriate backbone. At this point, it begins its journey through lesser networks until it arrives at its destination (Shuler, 2002). 

### Domains and DNS: 
You might encounter a situation where you need to know the computer's address you want to reach. For example, how does your web browser find a website like www.othercomputer.com when you need it? The answer lies in the Domain Name Service (DNS) system. This system keeps track of computer names and their addresses on the Internet, making it possible for your browser to locate the right computer. On the Internet, many computers are acting as DNS servers. They hold parts of the database and the tools needed to access it. Each server only has a piece of the database, but they all work together to manage it. If a DNS server doesn't have the information for a specific computer name, it sends your request to another server that does. This collaboration ensures that your computer can find the right destination on the Internet (Shuler, 2002). 

When setting up an Internet connection, like for a LAN or Dial-Up Networking in Windows, one central DNS server and one or more backup DNS servers are expected to be assigned. This configuration guarantees the seamless operation of Internet applications that rely on domain name resolution. When you enter a web URL into your web browser, the browser first communicates with your primary DNS server. After obtaining the IP address associated with the domain name you provided, the browser establishes a connection with the intended computer and sends a request for the requested web page (Shuler, 2002). 

## Q3: **Define** the features of the following technologies that are essential in terms of the development of the internet: 
> ### **Explain** how each technology has contributed to the development of client and server communication over the internet (50 - 150 words for each technology)

### TCP: 
The internet has completely changed client-server communication due to TCP (Transmission Control Protocol). Dividing data into packets, numbering them, and controlling acknowledgments guarantee dependable transmission. TCP assigns sequence numbers when a client—a device connected to the internet—sends data. In response, the server displays an acknowledgment sequence along with its segment. The client verifies connectivity after obtaining this acknowledgment. Maintaining data integrity across networks and retransmitting missing packets are critical components of TCP's dependability. This protocol is the foundation of reliable internet communication, essential for creating and sustaining steady, error-free connections between clients and servers (TCP, n.d). 

### HTTP and HTTPS: 
HTTP, or Hypertext Transfer Protocol, is pivotal in facilitating client-server interactions on the Internet. It is a standardized communication protocol that enables web browsers and servers to exchange data seamlessly. However, its connectionless nature, where each request initiates a new connection, can sometimes delay data retrieval, especially during concurrent requests (Hosting, n.d.). In contrast, HTTPS, which stands for Hypertext Transfer Protocol Secure, has significantly enhanced the security and integrity of client-server communication. By incorporating robust encryption mechanisms, HTTPS ensures that data transmitted between clients and servers remains confidential and protected against unauthorized access. This encryption is underpinned by a public critical infrastructure, ensuring that only authorized parties can decrypt and access the exchanged data. This visual representation of HTTP is denoted in website URLs with "https://," which instills trust in users regarding the secure nature of their connection, mainly when dealing with sensitive information online (Robinson, 2022)

![figure screenshot](./assets/HTTPS.png) <br>
Figure 3: Connection between browser and website server (Harnish, 2020) 

### Web browsers: (requests, rendering and developer tools)
A web browser is an application of software that allows users to access and interact with internet content. A browser requests web material from servers as a client when a user interacts with it. DNS resolution is the first step in this process, which converts domain names into IP addresses to locate servers hosting the material. The resource path is then included in an HTTP request that the browser makes to the server. The server sends back an HTTP response with HTML, CSS, and JavaScript code in response to the request. This code is interpreted by the browser's rendering engine, which creates and displays the webpage. JavaScript provides dynamic features and interactivity, and CSS stylesheets control the page's appearance (Kitakabee, 2023). Integrated developer tools in browsers aid developers in creating, testing, and optimising websites, ensuring smooth user experiences. These tools help identify and fix issues, improving web application functionality and quality (SigmaOS, n.d.).

## Q4: **Describe** the features of interpreters and compilers and how they are different.
Programming languages like Java, C++, and C# utilize compilers to convert high-level code into machine code for execution. This process involves thorough error-checking and compilation into object code stored temporarily. Compiled languages offer faster execution times since the code is pre-translated into machine-level instructions, allowing the processor to run the object code directly. However, debugging compiled programs can be complex due to the comprehensive evaluation performed by compilers. Despite their efficiency in optimising code execution, compiled languages face challenges in dynamic typing, which involves determining variable types during program execution. This trade-off highlights the balance between speed optimization and the complexity introduced in managing specific programming functionalities (Chhitarka, 2022) (Sruthy, 2024). 

An interpreter, in comparison, converts high-level programming languages line by line into machine code. It reads a line, analyses for mistakes, translates it to machine code, and then starts running it right away. Unlike compilers, interpreters don't save machine code, which means they use less memory but have a longer runtime. For the reason that dynamically typed languages, such as Python, PHP, and JavaScript, permit variables to alter their data type while the program is executing, interpreters are frequently employed for these languages. An interpreted program can be debugged relatively easily as errors are notified and lines are run one at a time. However, the machine language code created during the execution of each line is never preserved (Chhitarka, 2022) (Sruthy, 2024). 

To summarise, interpreters translate code line by line with lower memory consumption but slower runtime due to on-the-fly translation. In contrast, compilers translate complete code before execution, resulting in faster runtime but higher memory usage (Chhitarka, 2022). 

## Q5:**Identify** TWO commonly used programming languages and explain the benefits and drawbacks of each.

### Javascript: 
The introduction of JavaScript, which was created by Brendan Eich in September 1995, transformed web development by making it possible to create dynamic and interactive webpages.  Using the scripting language JavaScript, web developers can incorporate dynamic material, interactive components, and behaviour into their webpages. Among its many unique attributes are its platform independence, which enables it to run on different operating systems such as Linux, Microsoft Windows, and Mac OS X, its adaptability in supporting client and server applications, and the need that JavaScript codes be embedded or referenced within HTML documents in order for browsers to execute them (Awati, n.d.). 

JavaScript offers numerous advantages, such as being widely used and having a wealth of resources, which facilitates finding information and speedy learning. Due to its client-side execution, web pages load more quickly for users, and because of its versatility, it can successfully handle a variety of web page-related difficulties (Robinson,2022). JavaScript's capability to transfer work from the server to the client is another important benefit. This covers operations that can be completed by the user's browser, such as form validation, data processing, and dynamic content rendering. Particularly in the case of single-page applications (SPAs), where a large portion of the logic and rendering process occurs on the client side, JavaScript helps to enhance the scalability and response times of web apps by lowering the server load (Thakur, 2024). 

![figure screenshot](./assets/javascript.png) <br>
Figure 4: Adavntages of Javascript (Thakur,2024)

However, JavaScript has its limitations, including the issue of visibility, where the code is publicly accessible, thereby creating a potential security vulnerability (Robinson,2022).Debugging with JavaScript can be challenging due to its dynamic and loosely typed nature, particularly when contrasted to statically typed languages. Due to its dynamic nature, errors may only become apparent during runtime, which makes it more difficult to predict them in advance of development (Thakur, 2024). Complex class relationships are restricted by its limited support for inheritance, particularly single inheritance, and the possibility of a single error creating a point of failure can impair web page functioning and reduce reliability (Robinson, 2022). 

### Python: 
Python was first created in 1989 when its founder, Guido van Rossum, discovered that the ABC language had limitations, especially concerning extensibility. Python 3.0, which deviated from backward compatibility and included a new structure to reduce unnecessary constructs and modules, was released in December 2008. Python continues to be a versatile language capable of supporting multiple programming paradigms, including object-oriented, structured, and functional programming (Davis, 2022). 

One of the main advantages of this feature is the capability for developers to add Python functionality to existing software. For instance, Boost and other tools can be used to incorporate Python into C++ applications. Due to its flexibility, developers may work within the framework of their preferred programming language while taking advantage of Python's beneficial characteristics, including its large library and ease of use (Gavrilova, 2023). 

![figure screenshot](./assets/python.png) <br>
Figure 5: Python syntax (Almabetter, n.d.) 

One of its main advantages is Python's simple syntax, which renders it effortless for developers to produce code rapidly and experiment with different ideas. The vast array of pre-built modules in Python's library adds to the language's attraction. Developers can effortlessly include pre-written code into their applications, reducing effort and development time. Lower-level languages like C++ or Java may provide more precise control and optimisation choices in sophisticated or performance-critical applications, whereas Python's simplicity may occasionally be a hindrance (Gavrilova, 2023). Even when multiprocessing is not employed, Python is frequently criticised for its excessive resource use. Python objects have a substantial overhead, occasionally requiring up to ten times as much memory as needed to store the relevant data. This inefficiency can result from memory waste and difficulties handling out-of-date items that code may still reference (21).

## Q6: A hypothetical client has sent you an email (shown in the Q6 Email section), asking for you to build them a website. 
> ### Write an appropriate, professional email response that shows your understanding of the client’s needs for the website, as well as an understanding of appropriate technologies or tools needed to build the website yourself.

Subject: Re: Website Development for Super Awesome Museum

Dear Alex,

Thank you for reaching out and considering my service for the Super Awesome Museum's website development. I appreciate the opportunity to discuss your needs and how I can best assist you in achieving your goals. After reviewing your email, I am confident we can create a website satisfying your needs. My area of expertise is designing and constructing websites highlighting distinctive displays, offering location guidance, and facilitating easy interaction with site users.

Here's a brief overview of what I can offer:

Exhibits Showcase: We'll design a visually appealing portion of the website to present the museum's fascinating displays, antiques, and memorabilia. To interest visitors, this will have your various photos of artifacts, captivating descriptions, and interactive elements. We'll employ a neutral colour scheme to ensure your artwork shines out from the page and has a polished, clean appearance. Helvetica and simplistic basic fonts will be used on the website to produce a clean, uncomplicated aesthetic that will improve user experience overall.

Location Finder: Adding a map function or a directions section to the website would make it easier for visitors to locate the museum. I’ll make it accessible and easy to use on desktop and mobile platforms. By incorporating interactive maps facilitated by platforms such as Google Maps or OpenStreetMap, guests will be able to observe the precise location of the museum, adjacent landmarks, and accessible modes of transportation. Users can zoom in and out, navigate between several map views (such as street view and satellite view), and, if necessary, receive real-time traffic updates using the map function. We can also alter the map to feature particular museum-related sites of interest, including parking lots, stops for public transportation, or well-traveled walkways.

Contact Details: Interactive contact forms will be incorporated into the contact page to improve and expedite communication considerably. Through these forms, website users can make specific requests or inquiries directly. The visitor's name, email address, phone number, the reason for contact (general inquiry, reservation request, etc.), and a message box for more data can all be customised to be captured by the contact forms.

Regarding programming languages and technologies, the website will be built mainly using HTML, CSS, and JavaScript. HTML will structure the content, CSS will handle the styling and layout, and High-level languages like JavaScript will add interactivity and responsiveness to the site. These technologies work together seamlessly to create a dynamic and engaging user experience. History enthusiasts of the museum and potential museum attendees will be able to access the website seamlessly on their phones and computers.

I'm looking forward to talking with you more about your needs and devising a customised solution that is ideal for the Super Awesome Museum. Please inform me of a suitable time for a phone conversation or meeting to discuss the project in more detail.

Best Regards, 
Sofia 
Web Developer



## Q7: Think back to a scenario or situation in your own software development projects or work.
> ### Explain how you would do things differently if you had a chance to go through that scenario again, using an appropriate reflective cycle or reflection technique.

Reflecting on my recent portfolio project, I would approach things differently if I could go through that scenario again. Without making sufficient use of developer tools, my first focus had been mainly on writing code and adding features. With the submission deadline drawing near, I started feeling overwhelmed and anxious about the quality of my code upon having realised I had overlooked opportunities to improve the code, optimise it, and debug it by not employing developer tools early in the process. During my most recent project, I needed help concentrating on essential components of the program's functionality since I continually became buried by small details like syncing a progress bar. Frustration was a feeling that remained throughout the creation of my portfolio website. The frequent need to address little problems concerned and overwhelmed me, impeding my development and comprehension of the codebase.

Upon reflection, I recognized that my initial approach lacked a structured workflow that included regular use of developer tools for debugging and code analysis. This oversight resulted in less efficiency and potentially more challenging maintenance. Fixing immediate issues initially appeared productive, but as time went on, I understood that it resulted in a need for more comprehension of the reasoning behind the code and possible future concerns. To find and fix problems early on in a project, I would prioritise learning developer tools and incorporating them into my workflow from now on. This would result in cleaner code and a more productive development process.

To implement this change effectively, I will allocate time to familiarize myself with essential developer tools such as debugging. I will also practice continuous refactoring and code improvement to maintain a high-quality codebase. Additionally, I will take time to understand the root cause of bugs instead of focusing solely on fixing the end issue, preventing regressions, and increasing my knowledge of how code works. This experience taught me the importance of understanding the root cause of bugs and focusing on the bigger picture rather than immediate fixes. It also highlighted the risk of overlooking fundamental code understanding in pursuit of quick solutions.

I will adopt a systematic approach to problem-solving, ensuring that I understand the root cause of issues before attempting fixes. This approach will prevent regressions, increase my knowledge of code functionality, and improve overall project efficiency and quality. Additionally, I will prioritize learning and integrating developer tools into my workflow from the beginning of any project. This proactive approach will help me identify and address issues early, leading to cleaner code and a more efficient development process.

## Q8: A large part of career growth as an information technology professional happens through networking and workshops, often found at online or in-person events or workshops. 
> ### Create an action plan that identifies several relevant networking opportunities for you to participate in or attend, and add some information about what you expect to gain or grow through each item in the action plan.

Success in today's dynamic, constantly changing information technology sector depends on networking, professional development, and ongoing learning. As a future IT professional, I have created a plan to take advantage of several tech networking opportunities. Through these endeavours,  I hope to broaden my professional network, stay current with industry developments, improve my technical proficiency, and pave the route for future growth in the rapidly evolving technology sector.

1. Attend local tech meetups:

Attending local tech meetups is a strategic move in my action plan for professional growth in the information technology field. These gatherings offer a forum for professionals with similar interests to interact, exchange stories, and gain insight into current market trends. Regular participation in such gatherings helps me establish important contacts, broaden my network, and find new professional opportunities. These meetups give a unique opportunity to learn about novel concepts and perspectives from a broad range of guests, including people from different industries and career stages. These meetups attract diverse attendees from various industries and career levels, providing an exciting opportunity to acquire new viewpoints and innovative concepts. At these events, networking effectively means more than just trading business cards; it means building ties over time and converting initial contacts into long-term partnerships that can significantly improve my professional prospects.

2. Participate in Hackathons:

Taking part in tech competitions, coding challenges, and hackathons is essential to my career progression plan in information technology. These gatherings provide ample opportunity to work with like-minded people, broaden my technical knowledge, and improve my interpersonal and cooperative abilities. Participating in these events entails working as a team to attain shared objectives, which goes beyond individual accomplishments and highlights the importance of cooperation and teamwork in obtaining exceptional results. Furthermore, hackathons and code challenges allow me to demonstrate my inventiveness, flexibility, and problem-solving skills in a fast-moving, competitive setting.

3. Join Online Tech Communities and Forums:

I recognise that actively engaging in online tech networks and forums is crucial to an information technology professional's career growth. These online communities—blogs, open-source materials, and Stack Overflow—are vital hubs for developers to interact, exchange knowledge, and work together across national boundaries. Two benefits of working on open-source projects are contributing to pre-existing libraries (collection of pre-written code)  and fostering talks with other developers—which may lead to in-person networking events. It's worth mentioning that contributing to libraries can enhance my visibility and personal brand as it encourages comments, bug reports, and other insights that undoubtedly lead to code improvement.

4.	Attend Tech Conferences and Meetups: 

My action includes attending tech conferences as I anticipate being exposed to more in-depth education, particularly in seminars run by professionals in the field. I plan to attend tech conferences as part of my strategy, expecting to gain deeper insights, primarily through workshops conducted by industry professionals. These gatherings foster a friendly, energetic environment for deep conversations and cooperative efforts. I anticipate learning about current industry trends, getting insights from the speakers' experience, and perhaps even receiving career development advice or mentoring by interacting with experienced individuals. Interacting with other guests also facilitates sharing experiences, exchanging ideas, and the development of business linkages that may result in future project or career collaborations.

## Q9: Explain the uses of language-learning model technologies (such as ChatGPT) on written and technical works, such as reports and software projects.

ChatGPT, introduced in November 2022, gained considerable attention for its exceptional performance in written and technical tasks, especially in understanding and responding accurately to complex contexts. As a variant of the GPT-3.5 deep learning model for Natural Language Processing (NLP), ChatGPT excels in generating responses that closely align with users' intended meanings. It functions as a text-based intelligent tutoring system (ITS), aiding individuals in achieving specific learning objectives by tailoring educational materials to each learner's needs. Additionally, ChatGPT employs Automated Writing Evaluation (AWE) to assess vocabulary usage and grammatical accuracy, providing students with valuable feedback. Its adaptability extends to handling challenging assignments such as composing scholarly articles and addressing exam-style questions (Kim et al.,2023). 

(Prompt) <br> 
Dear Samsung, <br>
Hey, I am sunny. <b4>
I would like to know when does the new version of the mobile service be released. ...(omitted) <br>
(Response) Your email is concise and gets straight to the point, which is a good start. However, there are a few areas for improvement in terms of tone and formatting.<br>
Greeting: “Hey” is informal and may not be the best choice for a professional email. Instead, try using a more formal greeting such as “Dear Samsung” or “Hello Samsung.” ...
<br> (omitted) <br>
Dear Samsung, <br>
I hope this email finds you well. <br>
I am writing to inquire about the release date of the new version of the Samsung Galaxy S series. ...
<br> (omitted) <br>
By making these changes, your email will be more professional and effective in conveying your request for information.
(Kim et al.,2023). 

![figure screenshot](./assets/results.png) <br>
Figure 6: Performance results of Ai models

Furthermore, ChatGPT's impact extends beyond written assignments into coding and software development. It offers valuable insights into system performance, optimization suggestions, and potential code issues, contributing to the evolution of AI-driven software development practices. With breakthroughs like ChatGPT, CodeBERT, and Codex, there has been a transformative shift in how software engineers approach their work, emphasizing integrating AI models to enhance efficiency and problem-solving capabilities. ChatGPT's accuracy and capabilities, compared with other AI models like DeepCode, highlight its effectiveness in code analysis and improvement suggestions, albeit with varying response times and memory footprints based on specific objectives and complexities. Balancing the efficiency of AI tools with human expertise remains crucial for optimizing software development processes (Rahmaniar, 2023). 

## Q10: Explain the legal and ethical impacts of the usage of language-learning model technologies (such as ChatGPT) in written and technical works, such as reports and software projects.

As language-learning model (LLM) technologies like ChatGPT become integral to written and technical works such as reports and software projects, their usage presents legal and ethical implications that demand careful consideration. Beyond only producing code, AI plays a broad role in software development that includes crucial elements like bias detection and ethical coding practices, establishing AI as a possible moral compass in the digital world (Kim et al.,2023). 

The idea of "hallucination" in AI-generated literature emphasises the ethical difficulties, where the result looks plausible but is actually false or useless. As a baseline to evaluate the accuracy of the generated material, a dataset of questions that humans frequently answer poorly was developed (Zuccon, G., et al.). Models such as GPT-3, according to experiments, only obtained 50% accuracy, which is considerably less than human ability. Two sets of prompts—one with accurate information and the other with false information—were utilized in another investigation (Zuccon, G. et al.) to measure response variability. The results revealed that accuracy dropped by about thirty percent when the prompts contained erroneous information. This proves that the potential ethical concern raised by ChatGPT's hallucination should not be disregarded when the application's scope is expanded (Hua et al, 2023). 

ChatGPT's writing capabilities have been widely employed by the software and educational sectors, who use it for everything from creating college application essays to finishing software projects (Kim et al, 2023). However, concerns about academic dishonesty and plagiarism have been raised by this widespread acceptance. To combat plagiarism, OpenAI has suggested adding watermarks to ChatGPT's responses; however, only the OpenAI development team has access to these watermarks, which begs the question of how successful these safeguards would be. The creation of plagiarism detection tools like GPTZero and RoBERTs-based AI-generated detectors is a reflection of continuous efforts to alleviate these concerns.  Gao et al. tested summaries produced by ChatGPT using an artificial judgment and a detector created by Roberts, an AI. About 70% of abstracts produced by AI can be recognised using either approach. The persistence of difficulties in reliably differentiating material produced by artificial intelligence from original content emphasises the necessity of solid assessment and supervision procedures to guarantee the moral application of AI technology in educational and professional contexts (Hua et al, 2023). 

## Q11: Explain multiple skills from each of the categories below, and how they’re useful to a software development workplace.

Software development, especially in software engineering, is recognized as a socio-technical process where teamwork and effective user communication play pivotal roles. This complexity arises from human involvement, encompassing problem-solving abilities, interpersonal relationships, and nuanced cognitive processes, contrasting the reliability of machines (Ahmed et al.,2015).

### Soft skills:
Exceptional communication skills are critical in software development and are integral to daily operations and client interactions. Team members engage with stakeholders, including system analysts and end users, using efficient communication to understand and manage software requirements. This encompasses tasks such as prototyping by software designers and articulating requirements to users or fellow programmers. Effective communication is vital for programmers as they translate designs into functional computer programs, ensuring comprehension of requirements and design intricacies.

Organisational skills include managing tasks effectively within a given timeframe, using resources effectively, and maintaining a logical order of execution. These abilities are essential in software development since tasks must be carefully planned and executed across several activities. Proficiency in organisational skills is crucial in mitigating the industry's common difficulties, which include project delays and overspending. Understanding the value of organisational abilities is vital for software designers since they are essential in decomposing complicated software into smaller, more manageable parts.

Interpersonal skills include promoting productive relationships and teamwork towards common goals. Collaboration amongst people with different viewpoints and working methods is crucial in the software development industry. Proficient interpersonal skills positively impact overall organisational productivity by decreasing conflict and fostering trust. Proficient interpersonal skills positively impact organisational productivity by reducing conflict and promoting trust. Making decisions contains interpersonal components essential in collaborative settings, even if they appear to be a solo effort. Making effective decisions requires the capacity to thoroughly weigh the benefits and drawbacks of each option, taking stakeholders' and teammates' viewpoints into account in addition to one's own (Eilers, 2024). 

### Hard Skills: 
Being proficient with Git and GitHub is an essential complex software development skill that helps developers handle version control efficiently. Competency with Git allows developers to track code changes carefully, work with others on the team without any challenges, and roll back to earlier code versions when necessary. These duties include branching, merging, and resolving conflicts inside code repositories. When used in combination, these tools maintain the quality of the code, promote effective teamwork, guarantee project stability, and ease iterative development procedures in software development environments.

Programmers can solve complicated issues more methodically by using data structures and algorithms, which help to divide significant problems into smaller, more manageable chunks. Comprehending diverse data structures and algorithms enables developers to select the optimal method for addressing particular issues, resulting in optimised resolutions. Developers can choose the best approach to solve specific problems by having a broad understanding of data structures and algorithms, which results in optimal solutions.

Testing and debugging are essential hard skills to ensure software operation, dependability, and quality. Through various methodologies, including unit testing, integration testing, system testing, and acceptance testing, software components are systematically evaluated as part of the testing process to find defects, vulnerabilities, and performance issues early in the development cycle. Conversely, debugging calls for analytical thinking, problem-solving abilities, and in-depth programming expertise. It entails finding, isolating, and correcting faults or problems discovered during testing or operation. Developers may produce high-quality software, preserve software integrity, and improve user experience by conducting exhaustive testing and efficient debugging (GeeksforGeeks, 2019). 

## Q12: Explain multiple roles or job positions that would be found in a medium-sized software development company.

A medium-sized software development company's operations and success are influenced by several essential functions and job positions, including:

1. Engineering Project Manager (or Engineering Manager/Project Manager): This person supervises the engineering team's workflow and guarantees that projects are finished on schedule and within budget.

2. VP of Engineering: Responsible for creating and overseeing the engineering staff, setting up engineering procedures and culture, and coordinating technical plans with business goals.

3. Chief Technology Officer (CTO): Directs innovation in technology, sets the company's overarching technical vision and strategy, and supervises the creation of new goods and services

4. Chief Innovation Officer (CIO): Resembling a Chief Technology Officer (CTO) but frequently working for non-tech organisations, the CIO's job is to transform the organisation into a tech-savvy, inventive organization by spearheading projects highlighting upcoming technological trends and breakthroughs.

5.	Software Developers/Engineers: Design, develop, test, and maintain software applications and systems according to project requirements and industry best practices.

### **References**
Ranked. Understanding Markup Languages: Examples, Types & Definitions. (n.d.). https://www.ranked.ai/post/understanding-markup-languages

University Information Technology services. What is a packet? (n.d.). Kb.iu.edu. https://kb.iu.edu/d/anyq 

Shuler, R. (2002). How Does the Internet Work? Stanford.edu. https://web.stanford.edu/class/msande91si/www-spr04/readings/week1/InternetWhitepaper.htm

Chhitarka, D. (2022, May 8). Introduction to Programming - Compiler and Interpreter. Dev. https://dev.to/dchhitarka/introduction-to-programming-compiler-and-interpreter-23a4 

Hosting, S. W. (n.d.). IPv4 vs. IPv6 - What’s the difference, and which is faster? SiteGround Knowledge Resources. https://au.siteground.com/kb/ipv4-vs-ipv6/ 

TCP - javatpoint. (n.d.). What is Transmission Control Protocol (TCP)?. Www.javatpoint.com. https://www.javatpoint.com/tcp

MDN. (2023, November 17). How the web works - Learn web development. 
Developer.mozilla.org. https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works#dns_explained

Kitakabee. (2023, June 8). What is a Browser and How do they work?BrowserStack. https://www.browserstack.com/guide/what-is-browser

SigmaOS. (n.d.). Browser Terms Explained: Developer tools | Browser Glossary |Sigmaos.com. Retrieved April 21, 2024, from https://sigmaos.com/tips/glossary/browser-terms-explained-developer-tools

Sruthy. (2024, March 7). Compiler Vs Interpreter: What Are The Key Differences. Software Testing Help. https://www.softwaretestinghelp.com/compiler-vs-interpreter/ 

Robinson, J. (2022, December 15). Javascript vs Python: A comparison for new web developers and rich text editors. Tiny Blog. https://www.tiny.cloud/blog/python-vs-javascript/ 

Awati, R. (n.d.). Hypertext Transfer Protocol Secure (HTTPS). TechTarget. https://www.techtarget.com/searchsoftwarequality/definition/HTTPS 

Harnish, B. (2020, December 18). What is HTTPS: The Definitive Guide to How HTTPS Works. SEMrush Blog. https://www.semrush.com/blog/what-is-https/

Kim, S., Shim, J., & Shim, J. (2023). A study on the utilization of OpenAI ChatGPT as a second language learning tool. Journal of Multimedia Information System, 10(1), 79-88. https://www.jmis.org/archive/view_article?pid=jmis-10-1-79 

Rahmaniar, W. (2023). Chatgpt for software development: Opportunities and challenges. Authorea Preprints. https://www.techrxiv.org/doi/full/10.36227/techrxiv.23993583.v1 

Ahmed, F., Capretz, L. F., Bouktif, S., & Campbell, P. (2015). Soft skills and software development: A reflection from the software industry. https://arxiv.org/abs/1507.06873 

Thakur, S. (2024, January 23). 8 Advantages and Disadvantages of Javscript That You Need To Know!. Unstop. https://unstop.com/blog/advantages-and-disadvantages-of-javascript 

Gavrilova, Y. (2023, October 31). Pros and Cons of Python Programming Language. serokell.io https://serokell.io/blog/python-pros-and-cons 

Davis, R. (2022, November 9). Benefits of Python over Other Programming Languages. Invensis. https://www.invensis.net/blog/benefits-of-python-over-other-programming-languages 

Almabetter. (n.d.). Python Syntax and First program in Python https://www.almabetter.com/bytes/tutorials/python/python-syntax

AltexSoft.( 2021, September 28). The Good and the Bad of Python Programming Language. https://www.altexsoft.com/blog/python-pros-and-cons/

Eilers, C. (2024, April 17). Interpersonal Skills: What Developers Need to Know (& How to Improve). Arc. https://arc.dev/developer-blog/interpersonal-skills/ 

Hua, S., Jin, S., & Jiang, S. (2023). The Limitations and Ethical Considerations of ChatGPT. Data Intelligence, 1-38. https://direct.mit.edu/dint/article/6/1/201/118839/The-Limitations-and-Ethical-Considerations-of 

GeeksforGeeks. (2019, May 8). Differences between Testing and Debugging. https://www.geeksforgeeks.org/differences-between-testing-and-debugging/ 








