# UDAP Tools
This open source repository was created for community members to contribute resources
to help others implement the [UDAP](https://www.udap.org) Profiles for clients and servers.

[**UDAP Implementers Spreadsheet**](https://docs.google.com/spreadsheets/d/1awkXXQaeuRv5ysLo8R6f1fpfBlpTJGfSPK4xRjsai7M/edit#gid=1298836267)
Please add client, server, and identity services to the sheet above. Additional fields indicate use cases supported and deployment status.

UDAP Client Assets:

Key management

-Installing certificate into keystore

-Selecting a cryptographic library

DCR

Start by requesting server metadata:

    {
			"name": " https://stage.healthtogo.me:8181/fhir/r4/stage/metadata",
			"request": {
				"method": "GET",
				"header": [
					{
						"key": "Accept",
						"value": "application/fhir+json",
						"type": "text"
					},
					{
						"key": "Authorization",
						"value": "Bearer NSZuABXmmxK8HYAXaW0G_2sFNUBSU8cD",
						"type": "text",
						"disabled": true
					}
				],
				"url": {
					"raw": "https://stage.healthtogo.me:8181/fhir/r4/stage/metadata",
					"protocol": "https",
					"host": [
						"stage",
						"healthtogo",
						"me"
					],
					"port": "8181",
					"path": [
						"fhir",
						"r4",
						"stage",
						"metadata"
					]
				}
			},
			"response": []
		}
    
-Example Software Statement

-Signing a JWT for DCR

Use the private key to sign the JWT; the password may be needed by your library to activate the private key within the software

-Dynamic Client Registration Request

JWT-Based Client Authentication

-Example Assertion

-Signing a JWT for JBA

-Token request for Authorization Code Flow

-Token request for Client Credentials Flow

Tiered OAuth

-Hinting a user's identity service preference to the RS's AS

Server Validation

-See "JWT Processing" section of Server Assets

UDAP Server Assets:

Key management

-Simplified truststore management using trust bundles

-Truststore management using individual certificates

-JWT Processing

-Trust validation

UDAP Identity Service Assets:

UDAP Certification & Wallet Management Assets:

Secure storage of claims

UDAP Endorser Assets:

See Server Assets for key management
