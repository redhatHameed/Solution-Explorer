## API Designer, the Apicurito RESTful API visual designer


### Step 1: Importing APIs with Apicurio Studio


1. From Solution explorer application list select "API Designer"

3. Download the API example from https://raw.githubusercontent.com/redhatHameed/Solution-Explorer/master/Locations.json and save it

2. Click on Open API




* Creates a new activedocs
* activedocs name is required. `system-name` can be override with optional parameter.
* The swagger spec for the ActiveDocs is required. This is controlled with the
  positional parameter `spec`. It can be one of the following values:
  * *Filename* in the available path.
  * *URL* format (supported schemes are `http` and `https`). Toolbox will try to download content from given address.
  * Read from *stdin* standard input stream. This is controlled by setting
    the `-` value
* This is not idempotent command. If activedocs with the same name already exists, command will fail.
* Several other options can be set. Check `usage`

```shell
NAME
    create - Create an ActiveDocs

USAGE
    3scale activedocs create <remote>
    <activedocs-name> <spec>

DESCRIPTION
    Create an ActiveDocs

OPTIONS
    -d --description=<value>           Specify the description of the
                                       ActiveDocs
    -i --service-id=<value>            Specify the Service ID associated to
                                       the ActiveDocs
    -p --published                     Specify it to publish the ActiveDoc on
                                       the Developer Portal. Otherwise it
                                       will be hidden
    -s --system-name=<value>           Spe