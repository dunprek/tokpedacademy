# tokpedacademy



Mvvm 

 - testability
 - maintainablilty
 - doesnt hold ui reference in View model

 
 View model memiliki "SaveStateHandle" -- >> fungsinya mirip dengan savedInstanceState 
 
 why ;  viewmodel survive ONconfiguration change, dengan savestatehandle  - > kita bisa menghindari on memory yang 
 
 
 VIEwMODELFACTORY
 
 DIGUNAKAN JIKA VIEW MODEL MEMILIKI DEPENDENCY YANG LEBIH 
 
 khusus for my savestatehandle api, harus gunakan abstratsavedstateviewmodelfactory. 
 
 
 
 #Lifecycle aware observable
 bisa pake rxJavaObservable, androi livedata, kotlin flow 
 
 kenapa pake Livedata ? 
  ** Lifecycle owner - > bisa paek data--> untuk activity
  
  ** untuk fragment viewlifecycleOwner()
  define Livedata ituadalah data holder.. 
  
 
 setvalue () -> main thread
 atau post value() -> background thread 
 
 Livedata transformation. 
 
 livedata transformation tetep sama sesuai dengan yang observe
 
 switchmap - one on one 
 
 one to many transformatin
 )_- MediatorLiveData 
 
 viewmodel - > 
 
 
 model
 
 suspend func - > itu bisa kita set network dari couroutine data dari luar 
 
 Bastractsavestateviewmodelfactory
 
 1. tidak boleh ui reference di viewmodel
 2. jangan ada logic di ui make it dumb
 3. separate ui logic vbusines
 4. ui observe viewmodel 
 5. dont expse mutable 
 6. save instance state
 
 
 fun dengan suspend - > bisa jalan di background
 **Speech by Devara Akmal
 
 
 -----
 create movie app
 
 
 
