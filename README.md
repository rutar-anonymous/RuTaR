# RuTaR - A Dataset in Russian for Reasoning about Taxes

This a page with RuTaR dataset in 'rutar.xlsx' file and the sources used for RAG experiments in 'sources_dataset_for_rutar.json'.


Columns description in 'rutar.xslx':

'title' - name of the government document used for a question

'date_publication' - publication date of this document

'full_text' - document text

'question_letter' and 'answer_letter' - question and answer that were parsed from 'full_text' and were used to make new questions for LLM

'letter_type' - whether document is from Ministry of Finances or Federal Tax Service

'source_url' - url, where original document can be found

'question_for_llm' - question that we prepared for LLM based on the document contents

'found_sources' - reference sources that were extracted from the document. Their contents can be found in 'sources_dataset_for_rutar.json'

'true_answer' - correct answer to the 'question_for_llm', can be 'yes' or 'no' labeled as 1 and 0 respectively
