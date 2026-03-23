


powershell(use administrator) :

# 1. 在任意目录安装 global-agent
mkdir C:\Users\2551\proxy-fix
cd C:\Users\2551\proxy-fix
npm install global-agent

# 2. 设置环境变量（注意路径用双反斜杠或引号）
$env:GLOBAL_AGENT_HTTP_PROXY="http://127.0.0.1:7897"
$env:GLOBAL_AGENT_HTTPS_PROXY="http://127.0.0.1:7897"
$env:NODE_OPTIONS="-r C:\tools\proxy-fix\node_modules\global-agent\bootstrap"



# 再设置
$env:GLOBAL_AGENT_HTTP_PROXY="http://127.0.0.1:7897"
$env:GLOBAL_AGENT_HTTPS_PROXY="http://127.0.0.1:7897"
$env:NODE_OPTIONS="-r C:\Users\2551\proxy-fix\node_modules\global-agent\bootstrap"




$env:NODE_OPTIONS="-r C:\Users\2551\proxy-fix\node_modules\global-agent\dist\index.js"

node -e "fetch('https://ipinfo.io/json').then(r=>r.json()).then(j=>console.log('Country:', j.country))"

and if you can get

<img width="2258" height="193" alt="image" src="https://github.com/user-attachments/assets/a1be15fb-8e4e-4776-87b9-750ec9be6753" />


feel  good to use  `multicodex-proxy`

it help you to get your job done

<img width="1436" height="505" alt="image" src="https://github.com/user-attachments/assets/1816751f-5ea5-4013-b551-0289ad45fe2e" />


