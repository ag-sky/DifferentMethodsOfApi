# DifferentMethodsOfApi

# Traditional method using async class

new Async<Void, Void String>(){
override fun doInBackground(void ... voids){
fetchdatafromapi
}
override fun onPostExecte(string result){
update UI /// post on main thread.
}

}.execute();


# Using thread and handler

new Thread()( -> {
string data = fetchapi();
handle.post(->{
update ui
}

}.start()


# Rxjava

Observable<String> apicall = Observable.create(emitter- > {

emitter.next(fetchdatafromPI();
emitter.onComplete();
};

apicall.subsribeon(Schudler.io){
.observeon(Androidschudler.Mainthread)
.subscribe(textveiw.updateui
