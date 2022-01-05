# label-studio_setup
instructions to setup a label studio project 
```
https://labelstud.io/guide/install.html#Install-with-pip
```

In order to upload files from local directory , make sure you set the following environment to true .Refer to 
```
https://labelstud.io/guide/start.html#Set-environment-variables
```

# AWS integration
Webinar : https://www.youtube.com/watch?v=6e1OLH5Iw2U&t=2118s

Don't Dos:

1. Make sure set the region to US-East1
2.CORS config
```
[
    {
        "AllowedHeaders": [
            "*"
        ],
        "AllowedMethods": [
            "GET",
            "PUT",
            "POST",
            "DELETE"
        ],
        "AllowedOrigins": [
            "http://localhost:8080"
        ],
        "ExposeHeaders": [
            "x-amz-server-side-encryption",
            "x-amz-request-id",
            "x-amz-id-2"
        ],
        "MaxAgeSeconds": 3000
    }
]
```
