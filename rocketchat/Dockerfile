FROM rocketchat/rocket.chat:develop
LABEL org.freenas.interactive="false" \
      org.freenas.version=1 \
      org.freenas.upgradeable="true" \
      org.freenas.expose-ports-at-host="true" \
      org.freenas.autostart="true" \
      org.freenas.web-ui-protocol="http" 		\
      org.freenas.web-ui-port=3000 			\
      org.freenas.web-ui-path="web" 			\
      org.freenas.port-mappings="3000:3000/tcp" \
      org.freenas.volumes="[						                              \
          {								                                    \
              \"name\": \"/app/uploads\",					                        \
              \"descr\": \"Presistance directory\"		                        \
          }   \
       ]"                                                                                 \
       org.freenas.settings="[ 						                        \
          {								                                    \
              \"env\": \"ROOT_URL\",					                              \
              \"descr\": \"Database root PW\",				\
              \"optional\": true					                              \
          },								                              \
          {								                                    \
              \"env\": \"MONGO_URL\",					                              \
              \"descr\": \"Database username\",				\
              \"optional\": true					                              \
          }                                                                              \
      ]"            
