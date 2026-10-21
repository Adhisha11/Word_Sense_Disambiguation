===================================================
WORD SENSE DISAMBIGUATION (WSD) SYSTEM ANALYSIS REPORT
===================================================

1. SENSE INVENTORY ANALYSIS:
   - Total senses categorized for 'bank', 'bat', and 'light': 75 senses.
   - Systematically extracted lexical relations: synonyms, antonyms, hypernyms (superordinates), hyponyms (subordinates), meronyms, and holonyms.

2. DISAMBIGUATION EVALUATION:
   - Tested against 6 domain-diverse sample sentences.
   - The Lesk Algorithm successfully differentiated noun meanings (e.g., financial institution vs. river bank) and part-of-speech differences (e.g., noun 'light' as illumination vs. adjective 'light' meaning low weight) by computing overlap between context words and WordNet gloss/example definitions.

3. DELIVERABLES VERIFICATION:
   - 'sense_inventory.csv': Contains the structured dictionary mapping.
   - 'wsd_results.csv': Displays sample contextual prediction output.
