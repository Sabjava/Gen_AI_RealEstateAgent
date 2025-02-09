### **Project Summary: Personalized Real Estate Agent**

This project demonstrates the development of a **Personalized Real Estate Agent** using cutting-edge technology like Large Language Models (LLMs) and semantic search to generate, store, and personalize real estate listings based on buyer preferences. The project includes the following key components:

#### **1. Synthetic Data Generation - Generating Real Estate Listings with an LLM**
The project leverages a **Large Language Model (LLM)** to automatically generate diverse and realistic real estate listings. 11 listings were generated for houses in San Mateo county, CA, containing factual details such as property features (price, bedrooms, bathrooms, etc.), descriptions, and neighborhood insights. 

#### **2. Semantic Search - Creating a Vector Database and Storing Listings**
To enable semantic search functionality, the project demonstrates the creation of a **vector database**. I used Chroma database. The listings generated by the LLM are processed to create embeddings, which are then stored within the database. This system allows for efficient organization and retrieval of listings based on the semantic content rather than just keyword matching, improving the search experience for users. 

#### **3. Semantic Search of Listings Based on Buyer Preferences**
A key feature of the application is the ability to **semantically search listings** based on a buyer's preferences. When a user provides specific preferences (e.g., price range, neighborhood, number of bedrooms), the system performs a search through the vector database to return listings that best match the input criteria. The results are ranked based on how closely they align with the buyer's preferences.

#### **4. Augmented Response Generation - Logic for Searching and Augmenting Listing Descriptions**
The project also includes **augmented response generation**. After the listings are retrieved through the semantic search, the system uses buyer preferences to **augment the descriptions** of the listings. This enhancement tailors the listing descriptions, adding details that are aligned with the buyer's interests, while preserving the factual content of the original listings. 

#### **5. Use of LLM for Generating Personalized Descriptions**
Finally, an LLM is used to generate **personalized descriptions** for the listings. Based on the buyer's preferences, the system crafts unique and appealing descriptions for the properties, emphasizing the features that matter most to the buyer. These descriptions are designed to make the listings more attractive and engaging, providing a personalized experience for the user. Here is an example of such response:
```
Generated Prompt:
Human: 
You are an AI assistant that helps generate real estate listings based on provided data. 

### Context:
Luxurious modern home in the prestigious Palo Alto neighborhood. This 4 bed, 3 bath property boasts high-end finishes, a gourmet kitchen, and a spacious master suite.

---

Spacious family home in a quiet San Jose neighborhood. This 4 bed, 2 bath property features a large living room, updated kitchen, and a backyard with fruit trees.

---

Spacious family home in a quiet Redwood City neighborhood. This 4 bed, 3 bath property offers a large kitchen, formal dining room, and a backyard perfect for entertaining.

### Buyer Preferences:
- Budget: $1,900,000 max
- Neighborhood: Downtown San Mateo or close areas
- Bedrooms: At least 2
- Bathrooms: At least 2
- Would like easy access to public transportation
### Task:
Using the information above, answer the following question:
     A house with gourmet kitchen
### Guidelines:
- Use clear, concise language.
- Provide structured responses with details like **Neighborhood, Price, Bedrooms, Bathrooms, House Size, Description, and Neighborhood Description**.
- Maintain a professional yet engaging tone.
- craft a response that not only answers the question A house with gourmet kitchen, but also ensures that your explanation is distinct, captivating, and customized to align with the specified preferences. This involves subtly emphasizing aspects of the property that align with what the buyer is looking for.

Response: Based on your preferences, I have found a stunning property that perfectly fits your criteria. 

**Neighborhood:** Downtown San Mateo
**Price:** Within your $1,900,000 budget
**Bedrooms:** 4
**Bathrooms:** 3
**House Size:** Spacious
**Description:** This luxurious modern home in Downtown San Mateo offers a gourmet kitchen that is sure to impress any culinary enthusiast. With high-end finishes and top-of-the-line appliances, this kitchen is a chef's dream. The property features 4 bedrooms, 3 bathrooms, a spacious master suite, and a beautifully landscaped backyard perfect for entertaining. 
**Neighborhood Description:** Downtown San Mateo is a vibrant area with easy access to public transportation, trendy restaurants, shopping centers, and entertainment venues. This upscale neighborhood provides a perfect blend of convenience and luxury, making it an ideal location for those seeking a modern and sophisticated lifestyle. 

This property not only meets your requirements but also exceeds expectations with its gourmet kitchen and upscale features. It truly embodies the essence of luxurious living in the heart of Downtown San Mateo.
Sources: ['2', '9', '4']

```

### **Conclusion**
This project combines **LLM-generated listings**, **semantic search** powered by vector embeddings, and **augmented response generation** to create a highly personalized real estate search experience. It allows buyers to easily find listings that match their preferences and receive tailored property descriptions that appeal to their specific needs and desires.

### **Acknowledgements**
Thanks to the people who designed, made and teach this wonderful class! I am happy to be living in the era of LLMs. a It was a big help in this assignment. Thanks to the engineers who made tools like chatGPT possible which I used for this assignment
