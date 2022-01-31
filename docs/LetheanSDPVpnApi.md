# letheanSDP.letheanSDP/Api.LetheanSDPVpnApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Start-letheanSDPLetheand**](LetheanSDPVpnApi.md#Start-letheanSDPLetheand) | **GET** /letheand/start | 


<a name="Start-letheanSDPLetheand"></a>
# **Start-letheanSDPLetheand**
> void Start-letheanSDPLetheand<br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-DataDir] <String><br>
> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[-Version] <System.Nullable[Boolean]><br>



### Example
```powershell
$DataDir = "MyDataDir" # String | Returns the binary version
$Version = $true # Boolean | Returns the binary version (optional)

try {
    $Result = Start-letheanSDPLetheand -DataDir $DataDir -Version $Version
} catch {
    Write-Host ("Exception occurred when calling Start-letheanSDPLetheand: {0}" -f ($_.ErrorDetails | ConvertFrom-Json))
    Write-Host ("Response headers: {0}" -f ($_.Exception.Response.Headers | ConvertTo-Json))
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **DataDir** | **String**| Returns the binary version | 
 **Version** | **Boolean**| Returns the binary version | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

