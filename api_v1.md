# Introducing The Galaxy Harvester API
This REST API is designed to allow users to submit data to GH via other applications (eg client plugins for SWGEmu) using an API key generated for their registered username.

## Endpoints
- /api/v1/resources
    - Methods
        - GET
    - Serves
        - List of current (in spawn) resources
    - Required arguments
        - galaxy (int)
        - auth_key (string)
    - Optional arguments
        - TBC
    - example usage /api/v1/resources?galaxy=18&auth_key=blu3h4rv35t
- /api/v1/resources/resource
    - Methods
        - POST - Send new resource information
        - GET - Retrieve information for resource
        - PUT - Update resource information (eg. mark unavailable)
    - Serves
        - Specified resource name
    - Required arguments
        - galaxy (int)
        - auth_key (string)
        - name (string)
    - example usage /api/v1/resources/resource?galaxy=18&auth_key=blu3h4rv35t&name=doofer

## Usage


## Restrictions


## Responses