# Introducing The Galaxy Harvester API
This REST API is designed to allow users to submit data to GH via other applications (eg client plugins for SWGEmu) using an API key generated for their registered username.

## Endpoints
#### /api/v1/resources
- Methods
    - GET
- Serves
    - List of current (in spawn) resources
- Required arguments
    - galaxy (int)
- Optional arguments
    - verified (int, 0 = Default, Either, 1 = Unverified Only, 2 = Verified Only)
- example usage /api/v1/resources?galaxy=1&verified=2

#### /api/v1/resources/resource
- Methods
    - POST - Send new resource information
    - GET - Retrieve information for resource
    - PUT - Update resource information (eg. mark unavailable)
- Serves
    - Specified resource name
- Required arguments
    - galaxy (int)
    - name (string)
    - planet (optional for GET)
- Optional arguments
    - verified (int, 0 = Default, Either, 1 = Unverified Only, 2 = Verified Only)


- example usage /api/v1/resources/resource?galaxy=1&name=doofer

## Usage


## Restrictions


## Responses