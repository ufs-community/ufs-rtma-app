# ufs-rtma-app

A brief example to run ufs-rtma-app

## 1. clone the ufs-rtma-app repository

```
  git clone https://github.com/ufs-community/ufs-rtma-app.git
```
or
```
  git clone git@github.com:ufs-community/ufs-rtma-app.git
  ```

## 2. checkout ufs-rtma-app components
```
cd ufs-rtma-app
./manage_externals/checkout_externals
```

## 3. build ufs-rtma-app executables
```
cd ufs-rtma-app
./devbuild.sh 
```

## 4. generate a ufs-rtma-app workflow
```
cd ufs-rtma-app
source env/wflow_jet.env (use other wflow files for different platforms)
cd regional_workflow/ush
cp config.sh.3DRTMA_dev1 config.sh
vi config.sh (modify EXPT_BASEDIR, STMP, PTMP and other variables accordingly)
./generate_FV3LAM_wflow.sh
```

## 5. run the ufs-rtma-app workflow 

Follow the instructions printed out from step 4 to set up a cron job to run the generated ufs-rtma-app workflow

## 6. More
Reference the following documentation for more details

https://github.com/NOAA-GSL/ufs-srweather-app/blob/feature/RRFS_dev1/Setup-RRFS.md

https://github.com/ufs-community/ufs-srweather-app/wiki/Getting-Started

