# Home Match Application

## Project Introduction
Imagine you're a talented developer at "Future Homes Realty", a forward-thinking real estate company. In an industry where personalization is key to customer satisfaction, your company wants to revolutionize how clients interact with real estate listings. The goal is to create a personalized experience for each buyer, making the property search process more engaging and tailored to individual preferences.

## The Challenge
Your task is to develop an innovative application named "HomeMatch". This application leverages large language models (LLMs) and vector databases to transform standard real estate listings into personalized narratives that resonate with potential buyers' unique preferences and needs.

## Core Components of "HomeMatch"

### 1. Understanding Buyer Preferences
- Buyers will input their requirements and preferences, such as location, property type, budget, amenities, and lifestyle choices.
- The application uses LLMs to interpret these inputs in natural language, understanding nuanced requests beyond basic filters.

### 2. Integrating with a Vector Database
- Connect "HomeMatch" with a vector database, where all available property listings are stored.
- Utilize vector embeddings to match properties with buyer preferences, focusing on aspects like neighborhood vibes, architectural styles, and proximity to specific amenities.

### 3. Personalized Listing Description Generation
- For each matched listing, use an LLM to rewrite the description in a way that highlights aspects most relevant to the buyer’s preferences.
- Ensure personalization emphasizes characteristics appealing to the buyer without altering factual information about the property.

### 4. Listing Presentation
- Output the personalized listing(s) as a text description of the listing.

## Installation
Install the required packages::
``` python
!pip install -r requirements.txt
```

## Setup
1. Obtain an OpenAI API key and set it as an environment variable:

``` python
os.environ['OPENAI_API_KEY']="your-openai-api-key"
```

2. Prepare the real estate listings CSV file (listings.csv) and place it in the root directory of the project.

## Usage
Run the script.

The script will:
1. Ask a series of questions to gather the buyer's home preferences.
2. Perform a semantic search on the real estate listings to find the best matches.
3. Rank and score the recommended homes.
4. Print the personalized recommendations.

## Project Structure
- HomeMatch.ipynb: The main script that runs the AI real estate agent.
- listings.csv: The CSV file containing real estate listings.
- requirements.txt: A list of required Python packages.

## Example
Here's an example of how the output might look:

``` plaintext
Rank: 1
Score: 90
Neighborhood: Suburban Sanctuary
Price: $850,000
Bedrooms: 4
Bathrooms: 3
Size (sqft): 2,200
Description: Embrace suburban tranquility in this spacious 4-bedroom, 3-bathroom home surrounded by mature trees and green spaces. The open floor plan features a gourmet kitchen with granite countertops and stainless steel appliances, perfect for your culinary adventures. The cozy fireplace in the living room and the covered patio overlooking the landscaped backyard provide the ideal setting for relaxation and outdoor entertaining. Retreat to the master suite with a private bathroom and walk-in closet, offering a peaceful sanctuary within your home.
```
