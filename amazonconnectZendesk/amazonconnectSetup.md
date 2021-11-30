### Whitelist

Open the AWS Connect instance setup page and go to `Contact flows` tab then whitelist the created lambda

![env_variables](/images/lambda_whitelist.png)

## Contact Flow setup

As Shown in the below image add lambda and set contact attribute block.

![contact_flow](/images/zendesk_contactflow.png)

Open the lambda block and select the created lambda then change the Timeout to 8sec

![contact_flow](/images/zendesk_invokelambda.png)

Open the Set contact attribute block and give same Destination key and Attribute as `customerInfo` and type as `External`

>Note : Dont't change Destination key and Attribute value

![contact_flow](/images/set_contact_attribute.png)
