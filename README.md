# WEPPcloudR

## Test urls

https://dev.wepp.cloud/weppcloud/runs/lt_202012_26_Bliss_Creek_CurCond/cfg/WEPPcloudR/report.Rmd/

https://dev.wepp.cloud/weppcloud/runs/lt_202012_26_Bliss_Creek_CurCond/cfg/WEPPcloudR/hello_world.Rmd/?user=roger

https://dev.wepp.cloud/weppcloud/runs/lt_202012_26_Bliss_Creek_CurCond/cfg/WEPPcloudR/new_report.Rmd/?user=chinmay

https://dev.wepp.cloud/weppcloud/WEPPcloudR/proxy/comparative_report_input.Rmd/?user=chinmay&runids=portland_LittleSandy_HighSevS.202009.chn_cs110,portland_LittleSandy_ModSevS.202009.chn_cs110

https://dev.wepp.cloud/weppcloud/WEPPcloudR/proxy/comparative_report.Rmd/?user=chinmay&runids=portland_LittleSandy_HighSevS.202009.chn_cs110,portland_LittleSandy_ModSevS.202009.chn_cs110


## git credentials on linux

configure git to store credentials

https://stackoverflow.com/questions/35942754/how-can-i-save-username-and-password-in-git#35942890

Create a API token in github under Settings -> Developer Settings -> Personal Access Tokens to use as password

## geoserver access

1. connect to Uidaho VPN
2. ssh to setup port forwarding

```
> ssh -L 1337:localhost:1337 <username>@dev.wepp.cloud
```

3. open geoserver admin page in browser http://localhost:1337/geoserver/

## workaround for not starting after reboot

```
> sudo systemctl stop geoserver.service
> sudo systemctl start geoserver.service
```

can check status with

```
> sudo systemctl status geoserver.service
```
