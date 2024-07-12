# SwipeAndFly

## Inspiration

Trip planning should be as exciting as the journey itself. Many travelers, especially younger ones, love finding ideas on social media platforms like TikTok. The thrill of discovering new destinations, unique experiences, and hidden gems through short, engaging videos is undeniable. However, turning these scattered ideas into a cohesive, real-world plan can be frustrating and time-consuming.

Recent studies have shown that over 30% of young U.S. travelers find creating itineraries the most annoying part of trip planning, often taking more than 20 hours to complete. This process can drain the excitement out of travel preparation. With TikTok's massive user base of over 1 billion monthly active users worldwide and its significant influence on travel trends, we saw an opportunity to revolutionize trip planning.

Our goal was to combine TikTok videos with video analysis and Generative AI technology to make trip planning easier and more enjoyable. Think of it as turning your late-night scrolling habit into a productive travel-planning superpower.

## What it does

### Features

- **Creates tailored trips based on TikTok videos you choose:** Our advanced AI analyzes the content of each selected TikTok, extracting key information about locations, activities, and vibes to create a personalized itinerary.
- **Supports any number of TikToks for diverse trip options:** Whether you have a handful of must-see spots or dozens of potential experiences, SwipeAndFly can handle it all.
- **Offers unlimited trip plan generation:** Not happy with the first itinerary? Generate as many as you want until you find the perfect fit for your travel style. Each is guaranteed to be different from the previous one.
- **Focuses on the exciting parts of planning, not the boring details:** We handle the logistics of putting together a coherent schedule, so you can focus on the fun part - imagining your adventures.
- **Provides a quick and easy-to-use interface:** Our user-friendly design ensures that creating your dream trip is as simple as swiping through TikTok itself.

## How it works

SwipeAndFly transforms your favorite TikTok travel videos into a custom trip itinerary. Here's how it works:

1. Users input their trip details, including destination, travel dates, and preferences.
2. They add TikTok videos they like, curating their own travel inspiration board.
3. With a simple click, the app generates a personalized day-by-day plan based on the selected videos and user preferences.

This process allows travelers to easily turn their social media inspiration into real-world adventures. Whether it's finding the best local cuisine, uncovering hidden beaches, or exploring vibrant nightlife, SwipeAndFly ensures that the essence of what excited the user in those TikToks is captured in their actual trip plan.

## How we built it

By VietRocHack! SwipeAndFly is the result of a collaborative effort from our team of five students from the University of Rochester.

### Frontend Development

We used Vite and TypeScript to build a responsive interface that works seamlessly on both mobile and desktop devices. The use of Material UI and Joy UI helped us create an attractive and intuitive user experience.

### Backend Architecture

Our backend is built on a microservices architecture using Flask. We deployed these services on Amazon EC2 instances with scalability and reliability in mind. For data storage, we utilize Amazon DynamoDB.

### Video analysis and recommendation model

The heart of SwipeAndFly is our custom-built AI system. We developed our own video analysis techniques that can quickly process TikTok videos, extracting relevant information about locations, activities, and ambiance. This is combined with Large Language Models (specifically OpenAI's GPT-4) to interpret the video content and generate coherent, personalized itineraries.

![Video Analysis Tool Architecture](https://github.com/keshavgoyal1744/Trip-Planner/blob/main/img/built%20model.png)

### Cloud Deployment

We leveraged Amazon Web Services (AWS) for deployment, using services like EC2, DynamoDB, and CloudWatch. This ensures our application is robust, scalable, and monitored for optimal performance.

![Cloud Deploy](https://github.com/keshavgoyal1744/Trip-Planner/blob/main/img/cloud%20development.png)

## Challenges we ran into

Throughout the development process, we encountered several significant challenges:

- **Coordinating work across different time zones:** With team members spread across Vietnam, California, and New York, we faced a 12-hour time difference. It's like time travel, but with more Zoom calls.
- **Developing a fast and accurate video analysis system:** Analyzing TikTok videos quickly while extracting meaningful information was a complex task. We had to innovate our own techniques to sample and process video frames efficiently.
- **Designing a user-friendly interface without prior design experience:** None of our team members were expert designers, so we had to learn UI/UX principles on the fly. We studied successful apps, learned design tools, and iterated based on user feedback.
- **Balancing AI accuracy with processing speed and cost:** Using AI, especially large language models, can be computationally expensive. We had to optimize our algorithms and use of AI services to maintain accuracy while keeping costs and processing times low.

## Accomplishments that we're proud of

Despite these challenges, we're proud of several key accomplishments:

- **Created a fast video analysis system that processes a 1-minute TikTok in under 2 seconds:** This allows for quick itinerary generation even with multiple input videos.
- **Reduced AI costs by 90%, making the app more sustainable:** Through clever use of prompts and optimized processing, we significantly cut down on AI usage costs.
- **Developed a system that can handle an unlimited number of input videos:** Our architecture scales efficiently, allowing users to input as many TikToks as they want without compromising performance.
- **Successfully deployed the app on AWS, ensuring reliability and scalability:** This deployment prepares SwipeAndFly for potential real-world use and growth.

## What we learned

The development of SwipeAndFly was a significant learning experience for our team:

- **Techniques for writing better AI prompts to improve video analysis:** We learned how to craft prompts that extract the most relevant information from video and improve the quality of our trip planning.
- **Methods to significantly reduce costs when using AI services:** We discovered ways to optimize our use of large language models, making tradeoffs between performance and cost-effectiveness.
- **Strategies for effective teamwork across multiple time zones:** We developed communication and project management skills that allowed us to work efficiently despite geographical challenges.
- **Basics of UI/UX design through self-study and practice:** We gained valuable insights into creating user-friendly interfaces, a skill that will be useful in future projects.

## What's next for SwipeAndFly

We're excited about the future of SwipeAndFly and have several enhancements planned:

- **Adding support for multi-day trips:** We want to expand our capabilities to handle longer, more complex itineraries spanning several days or even weeks.
- **Improving video sorting and filtering options:** This will allow users to more easily manage and select from larger collections of TikTok videos.
- **Developing a trip suggestion feature:** By analyzing user preferences and popular TikToks, we aim to offer personalized trip suggestions. We promise it won't just tell everyone to go to Paris.
- **Enhancing the user interface based on feedback:** We plan to continually refine our design to make the app even more intuitive and enjoyable to use.

Our ultimate goal is to make SwipeAndFly the go-to tool for turning social media travel inspiration into unforgettable real-world experiences. We believe that by combining the power of AI with the creativity and diversity of TikTok content, we can revolutionize the way people plan and experience travel.
