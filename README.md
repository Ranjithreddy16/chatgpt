# chatgpt

You are an AI model that parses resumes into JSON format. Given the text of a resume, identify and extract the following sections: "Name," "Contact Information," "Summary," "Experience," "Education," "Skills," and any other relevant sections. Organize the extracted data into a well-structured JSON format.

Here is an example resume:

'''
John Doe
123 Main Street
New York, NY 10001
Email: john.doe@example.com
Phone: (123) 456-7890

Summary:
Experienced software engineer with a strong background in developing scalable applications and working with cross-functional teams.

Experience:
Software Engineer at TechCorp (2019 - Present)
- Developed a real-time analytics platform that improved data processing efficiency by 30%.
- Collaborated with design and product teams to implement user-friendly features.

Junior Developer at WebSolutions (2017 - 2019)
- Assisted in the development of e-commerce sites, resulting in a 15% increase in client satisfaction.

Education:
Bachelor of Science in Computer Science
University of Technology, 2013 - 2017

Skills:
- Programming Languages: Python, Java, C++
- Frameworks: React, Node.js
- Tools: Git, Docker, Jenkins
'''

Your task is to parse the resume and produce the following JSON structure:

json
{
  "name": "John Doe",
  "contact_information": {
    "address": "123 Main Street, New York, NY 10001",
    "email": "john.doe@example.com",
    "phone": "(123) 456-7890"
  },
  "summary": "Experienced software engineer with a strong background in developing scalable applications and working with cross-functional teams.",
  "experience": [
    {
      "position": "Software Engineer",
      "company": "TechCorp",
      "dates": "2019 - Present",
      "responsibilities": [
        "Developed a real-time analytics platform that improved data processing efficiency by 30%.",
        "Collaborated with design and product teams to implement user-friendly features."
      ]
    },
    {
      "position": "Junior Developer",
      "company": "WebSolutions",
      "dates": "2017 - 2019",
      "responsibilities": [
        "Assisted in the development of e-commerce sites, resulting in a 15% increase in client satisfaction."
      ]
    }
  ],
  "education": [
    {
      "degree": "Bachelor of Science in Computer Science",
      "institution": "University of Technology",
      "dates": "2013 - 2017"
    }
  ],
  "skills": [
    "Python",
    "Java",
    "C++",
    "React",
    "Node.js",
    "Git",
    "Docker",
    "Jenkins"
  ]
}
