## config file for labelling interface 
```
<View>
  <View>
    <Labels name="label1" toName="text">
      <Label value="TTI" background="#FFA39E"/>
      <Label value="VDT" background="#D4380D"/>
      <Label value="VNM" background="#FFC069"/>
      <Label value="TCO" background="#AD8B00"/>
      <Label value="VNM" background="#FFC069"/>
      <Label value="TAG" background="#D3F261"/>
      <Label value="VNU" background="#389E0D"/>
      <Label value="TUT" background="#5CDBD3"/>
      <Label value="TSP" background="#096DD9"/>
      <Label value="VLO" background="#ADC6FF"/>
      <Label value="TRL" background="#9254DE"/>
    </Labels>
    <Labels name="label2" toName="text">
      <Label value="TSS" background="#F759AB"/>
      <Label value="VID" background="#FFA39E"/>
      <Label value="TSP" background="#096DD9"/>
      <Label value="VLO" background="#ADC6FF"/>
      <Label value="TSP" background="#096DD9"/>
      <Label value="TDI" background="#AD8B00"/>
      <Label value="VNU" background="#D3F261"/>
      <Label value="TUT" background="#389E0D"/>
      <Label value="TSP" background="#096DD9"/>
      <Label value="TDI" background="#AD8B00"/>
      <Label value="VLO" background="#ADC6FF"/>
      <Label value="TDI" background="#AD8B00"/>
      <Label value="VID" background="#FFA39E"/>
    </Labels>
  </View>
  <Text name="text" value="$text" valueType="url" saveTextResult='yes' />
</View>


```

## AWS setup :
storage title : epi0
bucket name : lk-ner-0
prefix: epi0/page_txts_pro/


## Target setup : 
storage title : epi0-labels
bucket name : lk-ner-0
prefix: epi0/labels/

## Setup CORS config
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
            "http://localhost:8080",
            "http://localhost:8081",
            "http://localhost:8083"
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
