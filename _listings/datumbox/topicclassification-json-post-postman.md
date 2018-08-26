{
  "info": {
    "name": "Datumbox Identifies the Topic of the Document",
    "_postman_id": "00eb9c73-78a6-4324-a279-27d5a9c586c3",
    "description": "The Topic Classification function assigns documents in 12 thematic categories based on their keywords, idioms and jargon. It can be used to identify the topic of the texts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Adult Content",
      "item": [
        {
          "id": "15638dff-d214-48db-915a-6974a5aa7a40",
          "name": "AdultContentDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/AdultContentDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Adult Content Detection function classifies the documents as adult or noadult based on their context. It can be used to detect whether a document contains content unsuitable for minors."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76b8096d-bd93-423a-8a9d-63ad05e37481"
            }
          ]
        }
      ]
    },
    {
      "name": "Commercial",
      "item": [
        {
          "id": "9fd0322e-b0d7-4f70-86c0-641bdc8f46fa",
          "name": "CommercialDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/CommercialDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Commercial Detection function labels the documents as commercial or non-commercial based on their keywords and expressions. It can be used to detect whether a website is commercial or not."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af0acefe-3ae2-4e5c-8860-37e82a4b9bc1"
            }
          ]
        }
      ]
    },
    {
      "name": "DocumentsSimilarity",
      "item": [
        {
          "id": "ecb590d3-10e7-404b-be40-1e2138a08765",
          "name": "DocumentSimilarity",
          "request": {
            "url": "http://api.datumbox.com/1.0/DocumentSimilarity.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "copy",
                  "value": "{}",
                  "disabled": false,
                  "description": "The second text"
                },
                {
                  "key": "original",
                  "value": "{}",
                  "disabled": false,
                  "description": "The first text"
                }
              ]
            },
            "description": "The Document Similarity function estimates the degree of similarity between two documents. It can be used to detect duplicate webpages or detect plagiarism."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f958557-6199-4304-af29-ac534ee4bc52"
            }
          ]
        }
      ]
    },
    {
      "name": "Educational",
      "item": [
        {
          "id": "a77ccd4f-275c-41a3-a972-5099e97c0915",
          "name": "EducationalDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/EducationalDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Educational Detection function classifies the documents as educational or non-educational based on their context. It can be used to detect whether a website is educational or not."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14c4f5ab-9fa9-4b5d-a339-abe610381798"
            }
          ]
        }
      ]
    },
    {
      "name": "Gender",
      "item": [
        {
          "id": "471bb5e4-6399-42b7-a33d-8717a6e68fa6",
          "name": "GenderDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/GenderDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Gender Detection function identifies if a particular document is written-by or targets-to a man or a woman based on the context, the words and the idioms found in the text."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d58a059e-35ad-4d26-8151-cd6d1325c785"
            }
          ]
        }
      ]
    },
    {
      "name": "Keyword",
      "item": [
        {
          "id": "8b2626d8-ae34-438f-9a8e-3b34c7138bd6",
          "name": "KeywordExtraction",
          "request": {
            "url": "http://api.datumbox.com/1.0/KeywordExtraction.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "n",
                  "value": "{}",
                  "disabled": false,
                  "description": "The number of keyword combinations (n-grams) that you wish to extract"
                },
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Keyword Extraction function enables you to extract from an arbitrary document all the keywords and word-combinations along with their occurrences in the text."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b035731a-2586-446f-89aa-94478e14deb5"
            }
          ]
        }
      ]
    },
    {
      "name": "Language",
      "item": [
        {
          "id": "69f0a708-4626-4a33-a7b1-d65f7003b515",
          "name": "LanguageDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/LanguageDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Language Detection function identifies the natural language of the given document based on its words and context. This classifier is able to detect 96 different languages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed2dedb4-edce-4bb3-b088-ad6eb40f5ea2"
            }
          ]
        }
      ]
    },
    {
      "name": "Readability",
      "item": [
        {
          "id": "29ca9315-b2b0-43ba-b25e-97aba690340e",
          "name": "ReadabilityAssessment",
          "request": {
            "url": "http://api.datumbox.com/1.0/ReadabilityAssessment.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Readability Assessment function determines the degree of readability of a document based on its terms and idioms. The texts are classified as basic, intermediate and advanced depending their difficulty."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "780cb5e5-8320-440f-a111-b733a98adac2"
            }
          ]
        }
      ]
    },
    {
      "name": "Sentiment",
      "item": [
        {
          "id": "9e9d86fa-49df-4015-88c3-1b32e754fac8",
          "name": "SentimentAnalysis",
          "request": {
            "url": "http://api.datumbox.com/1.0/SentimentAnalysis.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Sentiment Analysis function classifies documents as positive, negative or neutral (lack of sentiment) depending on whether they express a positive, negative or neutral opinion."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e3a7af5-924f-4e87-94ff-d28b1549ec74"
            }
          ]
        }
      ]
    },
    {
      "name": "Spam",
      "item": [
        {
          "id": "076c9d8d-037b-445b-9b9f-32e01f0640f3",
          "name": "SpamDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/SpamDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Spam Detection function labels documents as spam or nospam by taking into account their context. It can be used to filter out spam emails and comments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a2efe6d-a6fd-4699-b76c-68561ab05d41"
            }
          ]
        }
      ]
    },
    {
      "name": "Subjectivity",
      "item": [
        {
          "id": "7969599b-2591-46e0-b48d-bf68b1908a39",
          "name": "SubjectivityAnalysis",
          "request": {
            "url": "http://api.datumbox.com/1.0/SubjectivityAnalysis.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Subjectivity Analysis function categorizes documents as subjective or objective based on their writing style. Texts that express personal opinions are labeled as subjective and the others as objective."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37c5b25b-a400-4d80-98e4-7154c7248fd3"
            }
          ]
        }
      ]
    },
    {
      "name": "Text",
      "item": [
        {
          "id": "bd4b5fa5-330a-4d15-8c2e-a8adb2026866",
          "name": "TextExtraction",
          "request": {
            "url": "http://api.datumbox.com/1.0/TextExtraction.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The HTML source of the webpage"
                }
              ]
            },
            "description": "The Text Extraction function enables you to extract the important information from a given webpage. Extracting the clear text of the documents is an important step before any other analysis."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8e74ce9-7d7d-46cb-85aa-cbcf7dfc824b"
            }
          ]
        }
      ]
    },
    {
      "name": "Topic",
      "item": [
        {
          "id": "3d9b03f2-e7ed-44ca-8ead-a20f90411fc3",
          "name": "TopicClassification",
          "request": {
            "url": "http://api.datumbox.com/1.0/TopicClassification.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Topic Classification function assigns documents in 12 thematic categories based on their keywords, idioms and jargon. It can be used to identify the topic of the texts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08444d7e-092f-40ea-afe5-cf95f5df2127"
            }
          ]
        }
      ]
    }
  ]
}