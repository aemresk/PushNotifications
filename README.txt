Android PushNotifications using PHP 

You should add firebase services AndroidManifest.xml 

 	<service
            android:name=".FirebaseMessagingService">
            <intent-filter>
                <action android:name="com.google.firebase.MESSAGING_EVENT"/>
            </intent-filter>
        </service>
        <service
            android:name=".FirebaseInstanceIDService">
            <intent-filter>
                <action android:name="com.google.firebase.INSTANCE_ID_EVENT"/>
            </intent-filter>
        </service>

And add this plugin your Gradle
    compile 'com.google.firebase:firebase-messaging:9.0.0'
    compile 'com.squareup.okhttp3:okhttp:3.2.0'

and this; 
apply plugin: 'com.google.gms.google-services'