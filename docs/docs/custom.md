# Custom Model

## Custom Models
In this section, contains a tabular representation of all the created custom model with their information.

![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/PredictCustomModels.png?raw=true)

Some of them are:
1. Name: Name of the custom model. 
2. Type: Type of thw custom model (Bulk Upload/Single Upload).
3. Status: The status of the run command on custom model.
4. Score: Score of the custom model.
5. Action: Click on action to Edit, Delete or Run the custom model.
6. Check multiple checkbox then click on **Run** button on top to run multiple custom models.
7. Click on **Run History** button on top. It's display tabular representation of run history.
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/PredictCustomModelRunHistory.png?raw=true)

## Steps to create a single upload custom model
This feature allows you to invoke your custom model service from SkyPoint Studio. We have a UI interface (like postman) which allows you to make HTTP calls to your service with all the required parameters and get the score from your service. The request parameters (url, body and headers) can be configured from UI. Request and Response body of the service is expected to be in JSON format. When running the model from Studio, platform makes an HTTP call to the service with required parameters and retrieves the output. You also need to specify the path of the score property in your JSON response.

The notation is very similar to Javascript notation of parsing properties.
1. Array properties indices start from 0 and are accessible with '[]' operator.
2. Object type properties are accessible with a '.' operator.

for eg. this is the JSON output of the service.
```json
{
    "category": 
    {
        "domain": "ecommerce",
        "priority": 1
    },
    "metrics": 
    [
        {
            "KPI": 
            {
                "conversions":[
                    {
                        "channel": "social",
                        "quantity": 3
                    }
                ]
            }
        },
        {
            "rate": {
                "score":[
                    7.8
                ]
            }
        }
    ]
}
```
The path property for score in this response is **metrics[1].rate.score[0]**.

1. Navigate to **Predict** > **Custom** and click on **New Workflow**.
![Alt text](https://github.com/skypointcloud/platform/blob/master/docs/doc_snippets/PredictCustomAddNewSingleUpload.png?raw=true)
2. Select single upload.
3. Enter the name of the web service.
4. Select URL method (GET/POST/PUT/DELETE).
5. Enter the web service URL.
6. Enter header key and value. Click on **Add Row** to create new header row.
7. Enter the web service body.
8. Enter the score path to map web service output.
9. Click on **Save**.


