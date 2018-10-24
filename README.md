<p align="center">
  <img src="http://lapisco.ifce.edu.br/wp-content/uploads/2018/03/cropped-LOGO-06.png" width="400" alt="accessibility text">
</p>

# VoIP with PJSip 
Into to voip with pjsip in python

## Prepare environments (with python2)
``` shell
$ pip install virtualenv
$ virtualenv -p my/path/to/python2 pjsip_env
```

## ADD to the environment variables
``` 
$ nano pjsip_env/bin/activate
```
#### COPY and PASTE into the file: 
```
export CFLAGS="$CFLAGS -fPIC"
```

#### SAVE: Press(Ctrl+X), Press(Y), Press(Enter)

## Install pjsip
``` 
$ git clone https://github.com/RaulMedeiros/voip_pjsip_python
$ cd voip_pjsip_python
$ ./configure
$ make dep
$ make
```

## Install python version of pjsip 
```
$ cd ./pjsip-apps/src/python/
$ python setup.py install
``` 
## Run sample
```
$ cd samples
$ python call.py
```


