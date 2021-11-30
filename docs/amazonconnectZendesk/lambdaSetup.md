## Lambda Setup

### Adding layers

Select `layers` on the sidemenu and click `Create Layer` button

![create_layer](/images/create_layer.png)

Download the layer files from <a href="https://lambda-layers-1h8d3.s3.ap-south-1.amazonaws.com/zendesk-integration.zip" target="_blank">S3 link</a>

![zendesk_layer_configuration](/images/zendesk_layer_configuration.png)

Fillout the fields as required and upload the ZIP file which downloaded before. Select `Node 14.x` as runtime and create the layer.

### Creating Lambda

Create new lambda function with basic execution permission with runtime `Node 14.x`  and copy the code from the <a href="https://github.com/Sandeza/arta-zendesk-installation" target="_blank">Github repo</a>.

> Note : Lambda and AWS Connect instance should be in same region

Add layers to lambda by selecting `Layers` under `Designer` tab and click `Add a layer` button as shown below

![layer](/images/zendesk_layer.png)
![add_layer](/images/zendesk_add_layer.png)

Select the layer which you have created before and the layer version then click Add button

![select_layer](/images/zendesk_layer_added.png)

Now the layer was added to lambda as shown below

![layer_added](/images/zendesk_layer_added_2.png)

> Note : To get Access Key and Integration ID, login to ARTA platform and integrate your Zendesk Account

Add the environment variables as shown in below image
> URL : devapi.arta.sandeza.io  \
> Note : Do not Include `https://` in beginning and  `/` at last

![env_variables](/images/zendesk_added_environment_variables.png)