# Chinese telemedicine-dialogue dataset(CTDD)
This dataset is used for Chinese medical dialogue named entity recognition task.
#Annotated entity type：
The entity types include the following
```
Diease, Symptom, Operation, Time, Pharmaceutical, examination
```
# Dataset format:
All the data is stored in a JSON file.There are 6 fields in the file. An example as follows:
```
    {
        "sentence_id": "1",
        "speaker": "患者",
        "sentence": "2020年9月因卵巢颗粒细胞瘤手术切除全子宫双附件大网膜，2022年3月发现复发，请医生给予治疗方案。",
        "BIO_label": "O O O O O O O O B-Diease I-Diease I-Diease I-Diease I-Diease I-Diease I-Diease O O B-Operation I-Operation I-Operation I-Operation I-Operation I-Operation I-Operation I-Operation I-Operation I-Operation I-Operation O O O O O O O ",
        "type": ["Diease","Operation"],
        "entity": ["卵巢颗粒细胞瘤","切除全子宫双附件大网膜"]
    },
    {
        "sentence_id": "2",
        "speaker": "医生",
        "sentence": "颗粒细胞瘤复发，建议尽量手术切除，术后补充化疗。",
        "BIO_label": "B-Diease I-Diease I-Diease I-Diease I-Diease I-Diease I-Diease O O O O O O O O O O O O O O O O O",
        "type": ["Diease"],
        "entity": ["颗粒细胞瘤复发"]
    },
```
# The JSON field details
```
sentence_id: The rotation of this sentence in this group's dialogue
speaker: The issuer of the current statement
sentence: Dialogue content
BIO_label: BIO annotation of the current statement
type: Entities Type
entities: Entities Words
```
# Final Words
This dataset currently provides 100 sets of dialogues for quality testing and public understanding, while the rest of the dialogue content is being prepared in a publicly available format. Stay tuned!<br>
Thanks for using our corpus! Please don't forget to let us know if our dataset advance the current state of the art forward in your Chinese natural language processing task.<br>
# Contacts
CTDD cannot be used for projects other than scientific research.<br>
Please contact us if necessary: yan_r79@126.com.
