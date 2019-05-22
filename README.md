# Improving Event Coreference Resolution by Modeling Correlations between Event Coreference Chains and Document Topic Structures


# STEPS
1) Run https://github.com/prafulla77/TAC-KBP-2017-Participation to extract event mentions and obtain pairwise score for coreference relations.
2) Run https://github.com/PrincetonML/SIF to generate pairwise sentence similarity scores.
3) Extract subevents using the patterns described in paper (a sequence of two or more verb event mentions that modify their parent verb with 'conj:and' or 'ccomp' dependency relations in a sentence are extracted as subevents).
4) Run new_test_ILP.py.


# Files format
- Coreference Scores: Run generate_coref_scores.py 
  OrderedDict([FileName:OrderedDict([Event_Key:OrderedDict([prev_event_key_1: score_1, prev_key_2:score_2)])...])

