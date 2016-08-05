# passwordless-ssh
# password less ssh

name=$1
host=$2
port=$3
echo "Exampel: passwordlessssh name host port"
cat ~/.ssh/id_rsa.pub | ssh -p $port $name@$host 'cat >> .ssh/authorized_keys'

