# genieacs-doc

* git clone https://github.com/genieacs/genieacs.git
* cd genieacs
* npm install 
* connects to mongodb
* create a database - use genieacs
* create a user - db.createUser( {user: "genieacs",pwd: "xxxxx", roles:[ {role: "root" , db:"admin"}, {role: "dbOwner" , db:"genieacs"} ] } )
* Update the MONGODB_CONNECTION_URL in the lib/config.ts to "mongodb://genieacs:xxxxx@host1,host2/genieacs?replicaSet=rs0&connectTimeoutMS=2000"
* sudo  mkdir /opt/genieacs
* sudo mkdir /opt/genieacs/ext
* sudo useradd --system --no-create-home --user-group genieacs
* sudo chown genieacs:genieacs /opt/genieacs/ext
* sudo vi /opt/genieacs/genieacs.env and add the GENIEACS_UI_JWT_SECRET=secret
* sudo chown genieacs:genieacs /opt/genieacs/genieacs.env
* sudo chmod 600 /opt/genieacs/genieacs.env
* npm run build

Reference links: https://github.com/genieacs/genieacs

https://docs.genieacs.com/en/latest/installation-guide.html#install-genieacs
