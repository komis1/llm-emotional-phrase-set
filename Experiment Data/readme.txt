### Experiment data file descriptors ###

==== participants.csv ==== 

pid: participant id
age: participant age
english: level of english proficiency NA=native speaker, NN=non-native without certification, A1-C2=CEFR classification
gender: f= female, m=male, o=other non-binary, u=prefer not to disclose
fingers: You usually type on your mobile with... i=index, t=one thumb, tt=two thumbs, gl=glide/swipe typing
ts: profile creation timestamp
autocorrect: Do you have Autocorrect enabled on your mobile keyboard? 1=Yes, 2=No
wordsuggestions: How often do you use Word Suggestions when you type messages? 1=Never, 5=All the time
timezone: automatically retrieved from browser
locale: automatically retrieved from browser
ptype: local participant (in the lab)
education: 1=high-school diploma, 2=vocational training diploma, 3=university degree, 4=postgraduate degree, 5=doctorate
occupation: 1=student, 2=self-employed, 3=employed, 4=home-maker, 5=retired, 6=unemployed

==== phrases.csv ==== 

id: serial entry number
pid: participant id
extype: Stimulus group, 1 = val+ ar+, 2 = val+ ar-, 3 = val- ar+, 4 = val- ar-, 5 = va0 ar0
orig_phrase: stimulus shown to participant
sub_phrase: phrase submitted by participant
effect: presentation effect for phrase (1=true) 
start: human-readable timestamp, time at first keyboard event entry
end: human-readable timestamp, time at last keyboard event entry
startts: unix timestamp, time at first keyboard event entry
endts: unix timestamp, time at last keyboard event entry


==== events.csv ==== 

id: serial entry number
pid: participant id
phrase:
event: KP=keypress, AC=autocomplete (more than 1 chars entered)
data: output character(s)
itype: input type as reported by browser (see https://w3c.github.io/input-events/#interface-InputEvent-Attributes)
ts: human-readable timestamp, time at keyboard event
extype: Stimulus group, 1 = val+ ar+, 2 = val+ ar-, 3 = val- ar+, 4 = val- ar-, 5 = va0 ar0
effect: presentation effect for phrase (1=true) 
tsunix: unix timestamp, time at keyboard event


==== questionnaires.csv ==== 

id: serial entry number
diff: time taken to complete questionnaire (from page load till submit)
pid: participant id
extype: Stimulus group, 1 = val+ ar+, 2 = val+ ar-, 3 = val- ar+, 4 = val- ar-, 5 = va0 ar0 
q1: How mentally demanding was the task? 0-20
q2: How physically demanding was the task? 0-20
q3: How successful were you in accomplishing what you were asked to do? 0-20
q4: How hard did you have to work to accomplish your level of performance? 0-20
q5: How insecure, discouraged, irritated, stressed, and annoyed were you? 0-20
q6: How much pleasure did the video at the start of the experiment make you feel? 0-100
q7: How stimulated did the the video at the start of the experiment make you feel? 0-100
q8: How much pleasure did you feel from the phrases presented to you? 0-100
q9: How stimulated did you feel from the phrases presented to you? 0-100

==== eda_means.csv & ecg_means.csv ==== 

id: participant id
conditionX_mean: mean signal value for all phrases in condition X
conditionX_q1: 1st quartile signal value for all phrases in condition X
conditionX_q2: 2nd quartile signal value for all phrases in condition X
conditionX_q3: 3rd quartile signal value for all phrases in condition X
conditionX_max: max signal value for all phrases in condition X
conditionX_min: min signal value for all phrases in condition X
X (conditions): 1 = val+ ar+, 2 = val+ ar-, 3 = val- ar+, 4 = val- ar-, 5 = va0 ar0

