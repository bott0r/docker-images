FROM rocketchat/rocket.chat
LABEL org.freenas.interactive="false" \
      org.freenas.version=1 \
      org.freenas.upgradeable="true" \
      org.freenas.expose-ports-at-host="true" \
      org.freenas.autostart="true" \
      org.freenas.port-mappings="80:3000/tcp" \
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
