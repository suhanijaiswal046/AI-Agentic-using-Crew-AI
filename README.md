
# CrewAI Gemini Travel Advisor ✈️

## Project Overview

The **CrewAI Gemini Travel Advisor** is an AI-powered travel planning project built using CrewAI and Google Gemini. It uses multiple AI agents to research travel destinations, estimate trip expenses, and generate a detailed 3-day travel itinerary.

The project helps users plan trips by considering historical places, weather information, hotels, public transportation, and budget constraints.

## Features

- Research historical sites and tourist attractions.
- Find hotel options near public transportation.
- Search for weather forecasts and travel information.
- Estimate hotel, food, transportation, flight, and attraction costs.
- Plan a detailed 3-day travel itinerary.
- Maintain the travel budget while planning.
- Use multiple specialized AI agents to complete tasks.

## Technologies Used

- Python
- CrewAI
- Google Gemini
- Serper API
- CrewAI Tools
- Google Colab

## AI Agents

### 1. Travel Researcher
Researches historical sites, weather information, hotels, and public transportation options for the selected destination.

### 2. Budget Planner
Estimates travel expenses, including accommodation, food, transportation, flights, and attractions, while considering the user's budget.

### 3. Itinerary Planner
Creates a 3-day travel itinerary based on the destination, available research, weather information, and budget constraints.

## How It Works

1. The user provides a destination and travel budget.
2. The Travel Researcher gathers relevant travel information.
3. The Budget Planner estimates the total travel expenses.
4. The Itinerary Planner creates a 3-day travel plan.
5. The crew generates the final travel recommendations.

The tasks are executed sequentially using CrewAI.

## Installation

Install the required packages:

```bash
pip install crewai crewai-tools
```

## API Configuration

This project requires API keys for Google Gemini and Serper.

If running in Google Colab, add your API keys to Colab Secrets:

- `geminikey` — Google Gemini API key
- `serperkey` — Serper API key

Never upload your API keys to GitHub.

## How to Run

1. Clone or download this repository.
2. Open `CREWAI_Gemini_travel_advisor.ipynb` in Google Colab or Jupyter Notebook.
3. Install the required dependencies.
4. Configure your API keys.
5. Run the notebook cells in order.
6. Provide the destination and budget when starting the crew.

Example input:

```python
result = await crew.kickoff_async(
    inputs={
        "destination": "London",
        "budget": "$1500"
    }
)

print(result)
```

The agents will research the destination, estimate expenses, and generate a 3-day itinerary.

## Example Output

For a trip to London, the project aims to generate:

- Recommended historical sites and tourist attractions.
- Hotel options near public transportation.
- Weather and travel information.
- Estimated travel expenses.
- A detailed 3-day itinerary.
- Budget-conscious transportation and accommodation recommendations.

Actual results depend on the available search results and API services. Verify prices, weather, and availability before travelling.

## Future Improvements

- Add a Streamlit web interface.
- Add travel dates and number of travellers.
- Improve currency conversion and budget calculations.
- Include source links for travel recommendations.
- Add personalized travel preferences.
- Improve error handling and validation.

## Author

**Suhani Jaiswal**


