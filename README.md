# 🎓 Smart College Campus Assistant — Multi-Agent AI with CrewAI

## 📌 Overview

The **Smart College Campus Assistant** is a multi-agent AI project designed to simplify college event planning and coordination. Built using CrewAI and Python, it combines three specialized AI agents to plan campus events, manage arrangements, and generate announcements for students.

The project integrates the Nexus API for LLM-powered text generation and the Open-Meteo API for weather information.

## 🤖 AI Agents

1. **Campus Event Planner** — Creates event schedules and resource lists.
2. **Campus Coordinator** — Summarizes weather information, seating requirements, and coordination arrangements.
3. **Communication Manager** — Generates clear announcements using information from the previous agents.

## 🛠️ Tools and Technologies

- Python
- CrewAI
- Nexus API
- Open-Meteo Weather API
- Requests
- Google Colab

## ⚙️ Key Features

- Sequential collaboration between three specialized AI agents.
- Six Python tools for event planning, resources, weather, seating, announcements, and coordination.
- Integration with an external weather API.
- Context sharing between agents to produce a combined event response.
- Input validation and error handling for invalid attendee counts.
- Testing with multiple event scenarios.

## 🔄 Workflow

1. The Event Planner generates a schedule and resource checklist.
2. Python tools retrieve weather data and calculate seating requirements.
3. The Campus Coordinator summarizes event arrangements.
4. The Communication Manager combines the available information into a final announcement.

## 🧪 Testing

The project includes tests for different events and attendee counts, along with an invalid-input test. The workflow was tested using an example event, **AI Innovation Day**, with 50 attendees.

## 🚀 How to Run

1. Open the notebook in Google Colab.
2. Install the required Python libraries.
3. Add your Nexus API key to Colab Secrets using the name `NEXUS_API_KEY`.
4. Execute the notebook cells in order.
5. Enter event details and review the generated planning and announcement outputs.

**Security:** Never commit API keys or other secrets to GitHub.

## ⚠️ Implementation Note

The selected Nexus model did not support native function calling. Therefore, Python executes the tools directly, while CrewAI agents use Nexus for normal text generation and process the results sequentially.

## 🎯 Learning Outcomes

- Understanding multi-agent AI systems.
- Creating specialized agents and chained tasks with CrewAI.
- Integrating external APIs into Python applications.
- Managing context and information flow between agents.
- Handling API errors and validating user inputs.

## 👨‍💻 Project Purpose

This project demonstrates how multi-agent AI and external tools can be combined to support practical college campus event planning and communication.
