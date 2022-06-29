# YAML

https://raw.githubusercontent.com/RodrigoMvs123/YAML/main/README.md



YAML ( Edit and View YAML - Online YAML Tools )


Yaml Tutorial | Learn YAML in 18 mins

XML 
JSON 

YAML is a data serialization language 
.yaml .yml

YAML ( Line Separation and spaces with indentation ) 
microservices:
app: user-authentication 
            port:9000
            version:1.0

XML ( Tags Angle Brackets ) 
<microservices>
<microservice>
<app> user-authentication </app>
<port>9000</port>
<version>1.0</version>
<microservice>
<microservices>

JSON ( Curly Brackets ) 
{
microservices: [
{
      app:”user-authentication”,
      port: 9000,
      version: “1.0”
}
]
}


Visual Studio Code
File ( Tutorial.yaml ) 

microservice: 
# comment here
 app: user-authentication
                port:9000
# second comment here 
                version: 1.7 
                deployed: true or false / yes or no / on or off 
app: shopping-cart 
     port: 9002 
     versions: [1.9,2.0,2.1]
 1.9 
2.0
2.1 

microservices:
user-authentication
shopping-cart 

Visual Studio Code
File ( Tutorial.yaml ) 

apiVersion: v1
kind: Pod
metadata:
   name: nginx
   labels:
   app: nginx 
spec:
   containers: 
name: nginx-container 
image: nginx 
            ports: 
containerPort: 80
            volumeMounts: 
name: nginx-vol
mountPath: /usr/nginx/html  
- name: sidecar-container
            image: curlimages/curl
           comand: [“/bin/sh”]
           args: [“-c” “echo Hello from the side car container; sleep 300” ]
   

Visual Studio Code
File ( Tutorial.yaml ) 

multilineString: > 
           this is a single line string,
           that should be all on one line.
           some other staff 

Visual Studio Code
File ( conf.yaml )
apiVersion: v1
kind: ConfigMap
metadata: 
   name: mosquitto-config-file
data: 
   mosquitto.conf:  | 
      log_dest stdout 
      log_type all
      log_timestamp true
      listener 9001

command:
- sh
- c
|
            http () { // ( Shell Script )
            local path=”${1}”
            set - -  -XGET - s - - fail
            curl - k “$@” “http://localhost:5601${path}”
}
           http “/app/kibana”


Visual Studio Code
File ( conf.yaml )

command:
-/bin/sh
-ec
>-
mysql -h 127.0.0.1 -u root -p$MYSQL_ROOT_PASSWORD -e “SELECT 1”



Visual Studio Code
File ( conf.yaml ) // PlaceHolder 

apiVersion: v1
kind:Service
metadata:
           name:{{.Values.service.name}}
spec:
     selector:
           app: {{.Values.service.app}}
     ports: 
protocol: TPC
port: {{.Values.service.port}}
targetPort: {{.Values.service.targetport}}


Visual Studio Code
File ( conf.yaml )

- - -

Visual Studio Code
File ( conf.yaml ) // PlaceHolder 

apiVersion: v1
kind:Service
metadata:
           name:{{.Values.service.name}}
spec:
     selector:
           app: {{.Values.service.app}}
     ports: 
protocol: TPC
port: {{.Values.service.port}}
targetPort: {{.Values.service.targetport}}

- - -

Visual Studio Code
File ( conf.yaml )

command:
-/bin/sh
-ec
>-
mysql -h 127.0.0.1 -u root -p$MYSQL_ROOT_PASSWORD -e “SELECT 1”



