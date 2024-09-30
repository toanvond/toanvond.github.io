---
title: Summer Research Internship at the University of Utah
type: post
date: 2024-08-20

# event: Hugo Blox Builder Conference
# event_url: https://example.org

# location: Hugo Blox Builder HQ
# address:
#   street: 450 Serra Mall
#   city: Stanford
#   region: CA
#   postcode: '94305'
#   country: United States

summary: "Developing Innovative Machine Learning Solutions in Medical Robotics: Predicting Tendon-Driven Robot Shapes with LSTM Networks and Automating Surgical Tasks"
# abstract: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellusac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum. Sed ac faucibus dolor, scelerisque sollicitudin nisi. Cras purus urna, suscipit quis sapien eu, pulvinar tempor diam.'

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
# date: '2030-06-01T13:00:00Z'
# date_end: '2030-06-01T15:00:00Z'
# all_day: false

# Schedule page publish date (NOT talk date).
# publishDate: '2017-01-01T00:00:00Z'

authors:
  - admin

tags: []

# Is this a featured talk? (true/false)
featured: false

image:
  caption: ''
  focal_point: Right

#links:
#  - icon: twitter
#    icon_pack: fab
#    name: Follow
#    url: https://twitter.com/georgecushen

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
---

## Introduction

This past summer, I had the incredible opportunity to work as an Undergraduate Research Assistant at the University of Utah's School of Computing, in the Utah Artificial Intelligence and Robotics in Medicine (ARM) Lab led by Dr. Alan Kuntz. For three months, I dove deep into the world of medical robotics, focusing on advancing techniques in tendon-driven robotic systems. This experience not only honed my technical skills but also allowed me to collaborate with a brilliant team of researchers. My experience at the University of Utah was both academically challenging and immensely rewarding, helping me grow as a researcher and as a professional.

## Predicting Tendon Robot Shape

<video controls>
  <source src="IMG_4543.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

The data collection process of the tendon robot shown above

One of the main projects I tackled was developing a model to predict the shape of a tendon-driven robot. Under the leadership of Dr. Kuntz, the lab has been exploring these robots, which are fascinating because their shapes can be manipulated by adjusting tendon displacements, which are 4 strings wrapped around the tendon robot with different strengths, functioning much like muscles in a human body, pulling and shifting to create movement. However, accurately predicting these shapes, especially in a 3D space, is a complex problem that is ongoing at the time.

During my internship, I was tasked with developing a machine learning model that could accurately predict the shape of the robot based on tendon displacement data. The problem had been partially addressed using other techniques, but we needed a more robust and efficient solution, especially for real-time applications.

To address this challenge, I employed Long Short-Term Memory (LSTM) networks — a type of recurrent neural network that excels at understanding sequences. My goal was to create a model that could predict the robot's shape as 3D point clouds based on the current tendon displacements. After rigorous testing and iteration, the model exceeded the previous learning-based techniques by 11% in terms of Chamfer distance, a metric used to measure the similarity between point clouds.

![Tendon LSTM](comparison.png "Deep Decoder Network (Left), the previous method, compared to LSTM (Right), where LSTM slightly performs better than the previous method")

## Collaborating on Bayesian Optimization for Surgical Retraction

Another exciting aspect of my internship was collaborating on a project that aimed to automate surgical retraction—a critical task in many medical procedures. Surgical retraction involves the use of tools to hold back tissue, providing the surgeon with better access to the area being operated on. Traditionally, this task requires manual input from surgical assistants, which can be imprecise and prone to human error. Our project sought to automate this process, using machine learning to optimize the positioning and force exerted by robotic retractors.

![dVRK](IMG_4532.png "da Vinci Research Kit (dVRK) robot")

The team I worked with adopted a Bayesian optimization approach to solve the problem, which is a powerful technique for finding the optimal set of parameters for a given system, particularly when the search space is large and complex. My role involved implementing different acquisition functions, which are used to determine the next point to sample in the optimization process. This approach led to significant improvements in detecting optimal attachment points for surgical tools, bringing us closer to fully automated surgical procedures.

![Simulation](IMG_4295.png "Experiment of the surgical retraction on the dVRK simulation")

By integrating various acquisition functions, we were able to find the function that improved the robot positioning and movement, allowing greater precision in revealing hidden areas of tissues more clearly.

## Reflections

Reflecting on my time in Dr. Kuntz lab, I can confidently say that this internship was one of the most formative experiences of my academic career. I was fortunate enough to work with a group of talented researchers who constantly challenged me to push my boundaries and think critically about the problems we were tackling.

The work we accomplished—developing predictive models for tendon-driven robots and automating surgical retraction—has the potential to make a real difference in the field of medical robotics. While there is still much more work to be done, I’m proud of the contributions I made and excited about the future of this research. I left the internship with a renewed passion for robotics and machine learning, and a deeper understanding of how these fields intersect in the context of healthcare.

Overall, my summer at the University of Utah, under the mentorship of Dr. Alan Kuntz, was an unforgettable experience that has shaped my approach to research and problem-solving. I am incredibly grateful for the opportunity to contribute to such impactful projects and to work alongside some of the brightest minds in the field. As I continue my academic journey, I look forward to building on the skills and knowledge I gained during this internship, and I am excited to see where this research leads in the future.

![Group photo](group_photo.jpg)