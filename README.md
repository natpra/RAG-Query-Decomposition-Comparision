# RAG-Query-Decomposition-Comparision

Overview

This repository consists of the use Retrieval-Augmented Generation (RAG) to compare Tesla and General Motors' approaches to manufacturing and production, with special attention to electric vehicles. By analyzing their manufacturing locations, production methods, and safety standards by using 10-K filings from both companies.

Data Sources
The code uses the following 10-K SEC filings:
•	Tesla: https://www.sec.gov/Archives/edgar/data/1318605/000162828024002390/tsla-20231231.htm
•	General Motors: https://www.sec.gov/Archives/edgar/data/1467858/000146785824000031/gm-20231231.htm

Main Question: "How do Tesla and GM's approaches to manufacturing and production compare, particularly for electric vehicles? Where are their vehicles produced? What are the safety standards followed in their vehicles?"

### Part 1: Standard RAG Approach
Implement a basic RAG pipeline to answer the main question without query decomposition.

### Part 2: Query Decomposition Approach
Implement a RAG pipeline that uses query decomposition to break down the main question into sub-questions before answering. 

## Comparison and Analysis

1. Overview of the Approaches
Simple RAG Approach:
•	The simple RAG approach combines information from the documents into a broader response to the main question. It retrieves relevant data from both Tesla and GM's 10-K filings and attempts to synthesize it into a cohesive answer.
•	The result is somewhat generalized. It provides a high-level comparison of Tesla and GM’s approaches to manufacturing, production, and safety standards but lacks specific details about their individual strategies or locations.
Query Decomposition (QD) Approach:
•	In contrast, the QD approach breaks the main question into smaller, focused sub-queries. Each sub-query zeroes in on a particular aspect of the question, such as the manufacturing approach, production locations, and safety standards for each company.
•	This approach results in more detailed, precise, and well-structured responses, as the information is targeted and relevant to each aspect of the main question.
2. Comparison of Results
a. Completeness and Focus
•	Simple RAG:
The simple RAG approach provides a broad overview but misses several crucial specifics. For example, it mentions that Tesla produces its vehicles using advanced manufacturing processes, but it does not provide any explicit information about Tesla’s Gigafactories or production locations beyond a general mention. GM's manufacturing is similarly vague, and both companies' safety standards are covered in a more general manner.
•	Query Decomposition:
The QD approach provides a detailed, specific answer to each sub-query. For instance, Tesla’s manufacturing approach is described in depth, covering its innovative techniques like in-house battery development and the Manufacturing Development Program. GM’s approach is similarly detailed, with specific mention of their "just-in-time" strategy and EV production at the CAMI Assembly. When it comes to production locations, the QD approach gives exact details about Tesla’s global production facilities (e.g., Gigafactory Shanghai, Fremont Factory) and GM’s facilities (e.g., CAMI Assembly, Ohio, Tennessee, Michigan). Regarding safety standards, the QD approach provides specifics about GM’s adherence to federal safety regulations and mentions Tesla’s regulatory scrutiny related to driver assistance systems, even though it lacks specific standards.
b. Clarity and Structure of Answer
•	Simple RAG:
The answer from simple RAG is generally coherent, but the lack of depth and clarity in certain areas (such as detailed locations or safety standards) makes it harder to fully understand the nuanced differences between Tesla and GM. It’s a broad stroke comparison, which is useful for a general overview but not for detailed analysis.
•	Query Decomposition:
The QD method provides a much clearer and more structured answer. Each sub-query is answered distinctly, giving a clear, segmented look at Tesla’s and GM’s respective strategies. For example, the manufacturing approaches of the two companies are well differentiated—Tesla’s emphasis on innovation and GM’s focus on scalability and traditional methods are clearly laid out. The same structure is applied to production locations and safety standards, making the comparison easy to follow.
c. Depth of Information
•	Simple RAG:
The RAG approach is broad and general, offering high-level comparisons but lacking deeper insight. While it mentions key facts, such as Tesla’s use of lithium-ion battery packs and GM’s commitment to EV production, it doesn’t go into the same level of depth. For example, GM’s safety standards are discussed briefly, without diving into specifics like how GM complies with the Safety Act of 1966 or its evaluation via NCAPs.
•	Query Decomposition:
The QD approach offers a deeper exploration of both companies. For instance, Tesla’s advanced manufacturing techniques (like battery integration into vehicle structures) and its global footprint are discussed in more detail. Similarly, GM’s "just-in-time" approach and its EV production at the CAMI Assembly are elaborated upon, providing richer insights. Safety standards are also explored more thoroughly, particularly GM’s adherence to federal safety regulations and Tesla’s scrutiny of driver assistance systems.
3. Which Approach Produced a Better Answer and Why?
Query Decomposition (QD) is the superior approach for answering this particular question for several reasons:
•	Targeted Focus: The QD approach breaks the question into smaller, more manageable pieces, allowing for a deeper dive into each aspect of manufacturing, production, and safety. This results in answers that are both comprehensive and specific, ensuring that no key details are overlooked.
•	Clarity and Structure: By isolating each part of the question, the QD approach makes the comparison between Tesla and GM easier to follow. The clear segmentation of information allows the reader to see the differences between the two companies with ease.
•	In-Depth Information: The QD approach provided more detailed and insightful responses, offering specific examples and deeper analysis of both companies’ strategies. This helps create a more complete and accurate picture of how Tesla and GM compare.
The Simple RAG approach, while effective for a broad overview, did not provide enough specificity or depth in key areas, particularly when discussing production locations and safety standards. For a detailed and structured comparison, the QD approach excelled in providing relevant, detailed answers.

Suggestions for Future Improvements
While the QD approach proved to be more effective, a few improvements could enhance the process further:
•	Refining Sub-Queries: Some sub-queries, like those about safety standards, could be refined to focus more specifically on each company’s safety measures, technological innovations, and their impact on consumer safety.
•	Additional Sources: In future iterations, incorporating additional data sources (e.g., interviews, press releases, or other corporate documents) could help provide an even more well-rounded analysis, particularly in areas where 10-K filings might lack detail, such as specific safety technologies or production challenges.
•	Hybrid Approach: A hybrid model that combines the comprehensive nature of simple RAG with the depth of query decomposition could prove effective in balancing high-level context with detailed insights.
Conclusion
In conclusion, while both approaches have their strengths, the Query Decomposition (QD) method provided a more thorough and structured analysis. By breaking the question into smaller sub-queries, you were able to extract more detailed, relevant, and specific information, leading to a better comparison of Tesla’s and GM’s manufacturing approaches. This approach is more suitable when a nuanced and in-depth analysis is required, as it enables a detailed examination of each aspect of the main question.
