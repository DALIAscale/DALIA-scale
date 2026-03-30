# DALIA Core Specification (v1.0)

The DALIA scale measures AI intervention based on cognitive load, intention, and control across the three phases of the creative design process: Ideation, Execution, and Refinement.


## 6 Levels of DALIA

| DALIA Level | Category Name | Summary | Who finds the idea? | Who creates it? | Who curates & finishes  it? | Real life examples |
| --- | --- | --- | --- | --- | --- | --- |
| D0 | Manual (No AI) | 100% Human. AI is not used at all. The creative process is performed entirely manually. | Human | Human | Human | Painting on a real canvas; writing an essay from scratch; taking a film photograph. |
| D1 | Tool-Assisted | Human. AI analyses in the background. Human acts and decides. | Human | Human | Human (with analytical AI tools) | Facial recognition groups photos in an album; tempo/key detection in audio software; code linter flags errors without rewriting. |
| D2 | AI-Augmented | Human. AI intervenes in the creation of specific, small elements but doesn't change the meaning of the work. | Human + limited inputs from AI | Mostly Human (Generative AI fills small gaps) | Human | Using generative fill to remove a small imperfection from an image; asking AI to rephrase one clunky sentence. |
| D3 | Guided Creation | Human & AI Teamwork. The human and AI act as creative partners. | Human + creative inputs from AI | Human & AI (AI builds a base, human changes it heavily) | Human (does major edits and assembly changing the meaning of the AI input) | Human-made art based on generated material; co-writing a story line-by-line with a chatbot. |
| D4 | AI-Generated (Human Directed) | Human as Art Director. The AI does the creative and production work, while the human gives orders and judges the results. | AI under Human direction | AI (creates the bulk of the work) | Human (picks the best option or makes tiny adjustments) | Using a generated image as-is; having an AI write a full blog post and only changing a few words; vibe coding without human code interventions. |
| D5 | Fully Autonomous | 100% AI. The human just presses "start" or sets up a system. The AI systems operate independently to handle the task. | AI | AI | None (used exactly as the AI made it) | A news bot that automatically writes and posts updates on social media; an AI generating endless background music on its own. |


_(Note: We will expand this document through community RFCs to include specific criteria for visual arts, music production, software engineering, and literature)._

## Notes
1. The scale reflects a shift in AI's role: at lower levels (D0-D1), AI operates analytically, helping humans perceive and decide. From D2 upward, AI becomes generative, producing content that the human then shapes or accepts.
2. DALIA classifies the production workflow, not upstream preparation. Custom model training, dataset curation, or fine-tuning are not factored into the level. A practitioner who trains a LoRA for weeks then generates in one click is rated on the generation act itself. This specific scenario may be adressed in future revisions. 
3. When a project combines multiple DALIA levels across its components, the overall classification defaults to the highest level present. A feature film shot on analog cameras but incorporating AI-generated visual effects is classified at the level of those effects, not the live footage. Where granularity matters, an optional compound notation may specify per-component levels (e.g. D2, with D4 elements for visual effects). The default rule remains the maximum.
4. DALIA does not evaluate the ethics of the AI tools used. Some models are built with more ethical approaches than others (training data consent, environmental impact, labour practices), and these considerations matter. However, they fall outside the current scope of the scale. DALIA measures the degree of AI involvement in the creative process, not the nature or provenance of the AI itself. Future versions may explore ways to integrate ethical dimensions as a complementary axis.

## References
**1. Haase, J., & Pokutta, S. (2024). _Human-AI Co-Creativity: Exploring Synergies Across Levels of Creative Collaboration_.** _Contribution to DALIA:_ This research introduced a four-level taxonomy of human-AI interaction, ranging from a "Digital Pen" to an "AI Co-Creator". It fundamentally inspired the progression of agency within the DALIA scale, demonstrating how AI evolves from a passive execution tool into an active, synergistic partner in the creative process.

**2. Wu, Z., et al. (2021). _AI Creativity and the Human-AI Co-creation Model_.** _Contribution to DALIA:_ By dividing the Human-AI co-creative design process into distinct, iterative stages (including perception, expression, construction, and testing), this work provides the theoretical foundation for evaluating AI's intervention not as a whole, but across the separate dynamics of Ideation, Execution, and Refinement.

**3. Hutson, J. (2025). _Human-AI Collaboration in Writing: A Multidimensional Framework for Creative and Intellectual Authorship_.** _Contribution to DALIA:_ This paper explicitly addresses the limitations of evaluating AI involvement on a simple sliding scale from "none" to "complete" `. It validates DALIA's shift away from a flawed percentage-based metric toward a multidimensional matrix assessing content generation, structural assistance, and creative input `.

**4. Lamers, M.H. (2025). _Introducing a scale for AI's artistic autonomy_.** _Contribution to DALIA:_ This research proposes a specific taxonomy for levels of automated artistic autonomy based on the division of responsibilities. It confirms the necessity for an operational scale that clarifies the autonomy given to generative AI systems and who is ultimately responsible for the steps within an artistic scenario.

**5. Salma, Z., et al. (2025). _Designing Co-Creative Systems: Five Paradoxes in Human–AI Collaboration_.** _Contribution to DALIA:_ By analyzing the irreducible paradoxes of co-creation (such as the tension between human control and machine serendipity), this framework justifies the necessity of identifying the "Locus of Control" (e.g., human as a director or curator) to understand how creative agency is maintained when using generative tools.

**6. SAE International (2021). _Taxonomy and Definitions for Terms Related to Driving Automation Systems (SAE J3016)_.** _Contribution to DALIA:_ Although originating from the automotive industry, this internationally recognized standard establishes the definitive 6-level architecture (Levels 0 to 5) for measuring the transfer of tasks from human to machine \`\`. It provides the structural benchmark and logical progression used to build the DALIA levels.
