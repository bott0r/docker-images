FROM bitnami/mongodb:latest
LABEL org.freenas.interactive="false" \
      org.freenas.version=1 \
      org.freenas.upgradeable="true" \
      org.freenas.expose-ports-at-host="true" \
      org.freenas.autostart="true" \
      org.freenas.port-mappings="27017:27017/tcp" \
      org.freenas.volumes="[						                              \
          {								                                    \
              \"name\": \"/bitnami/mongodb\",					                        \
              \"descr\": \"Presistance directory\"		                        \
          }   \
       ]"                                                                                 \
       org.freenas.settings="[ 						                        \
          {								                                    \
              \"env\": \"MONGODB_ROOT_PASSWORD\",					                              \
              \"descr\": \"Database root PW\",				\
              \"optional\": true					                              \
          },								                              \
          {								                                    \
              \"env\": \"MONGODB_USERNAME\",					                              \
              \"descr\": \"Database username\",				\
              \"optional\": true					                              \
          },								                              \
          {								                                    \
              \"env\": \"MONGODB_DATABASE\",					                              \
              \"descr\": \"Database name\",				\
              \"optional\": true					                              \
          }\
      ]"                                                                                  
