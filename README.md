# Injected Root Files Manager  

<img src="https://i.ibb.co/MZjhPmG/20250121-184657.jpg" alt="Koshur Boii Injected Root Files Manager" style="width: 100%; height: auto; border: 0;"/>

An advanced tool for developers, designed to access private app folders in Android apps that are normally difficult for regular users to access without root permissions. However, with this tool, you can efficiently access and manage those folders on **non-rooted devices** to inspect and validate root-level file encryption and security. Created by Abrar Hussain Beigh (Koshur Boii), this tool seamlessly integrates with APKs to ensure comprehensive security testing.

---

## **Overview**  
The Injected Root Files Manager is a powerful and efficient tool for developers aiming to test their apps for security vulnerabilities. It enables inspection of root-level directories on **non-rooted devices**, ensuring sensitive data is encrypted and protected. This tool is tailored for testing and debugging during the development lifecycle.

---

## **Purpose**  
- Validate the security of Android apps by inspecting root directories on **non-rooted devices**.  
- Ensure sensitive data is encrypted, hidden, and inaccessible to unauthorized users.  
- Test compliance with data protection and privacy standards.  

---

## **Features**  
- **Direct Root Folder Access**: View and manage root-level files effortlessly.  
- **Lightweight Integration**: Bind with APKs or use as a standalone library.  
- **Developer-Friendly Interface**: Intuitive design for seamless use during development.  
- **Multiple Usage Modes**:  
  - Bind with your APK and access via launcher activity.  
  - Use it as a standalone library by integrating it into your app’s codebase.  

---

## **How to Use**

### 1. **Patch File Method**  
- [Download Patch File](https://github.com/koshurboii/Injected-Root-Files-Manager/releases/download/v1.0.0/patch_koshurboii_InjectedRootFilesManager.zip)  
- Use the downloaded patch file with an APK editor on your mobile device.  
- Bind the patch file with your APK to gain root file access and perform vulnerability testing.

### 2. **Library Integration**  
- Download the source code of the library.  
- [Download source code](https://github.com/koshurboii/Injected-Root-Files-Manager/archive/refs/tags/v1.0.0.zip)  
- Integrate the library into your app to manage root-level directories.

### 3. Update `AndroidManifest.xml`
- Add necessary permissions and activities:

```xml
<uses-permission android:name="android.permission.SYSTEM_ALERT_WINDOW"/>
<uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
<uses-permission android:name="android.permission.MANAGE_EXTERNAL_STORAGE"/>
```

-  **Set `org.koshurboii.InjectedRootFilesManager.MainActivity` as  Launcher Activity** and add `org.koshurboii.InjectedRootFilesManager.KoshurboiiEditPreferenceActivity` : 

```xml
    <activity
        android:name="org.koshurboii.InjectedRootFilesManager.MainActivity"
        android:exported="true">
        <intent-filter>
            <action android:name="android.intent.action.MAIN"/>
            <category android:name="android.intent.category.LAUNCHER"/>
        </intent-filter>
    </activity>

    <activity
        android:name="org.koshurboii.InjectedRootFilesManager.KoshurboiiEditPreferenceActivity"/>
```

- **Add `<meta-data>` to the App's Main Entry Activity**

- To add the `<meta-data>` to the **main entry activity** of your app (where the user lands when opening the app), use the following XML configuration:

```xml
<activity 
    android:label="Your App Name"
    android:name="com.example.yourapp.MainActivity">
    
    <meta-data
        android:name="role"
        android:value="entry"/>
</activity>
```

---

## **License**  
This project is licensed under the **MIT License**. For more information, check the `LICENSE` file included with the project.  

---

## **Disclaimer**  
This tool is intended **exclusively for developers and advanced users** to test their own apps and systems responsibly. The author is not liable for any misuse or damage caused by improper usage.  

---

## **Contact**  
Need a custom solution or assistance with app security testing? Feel free to get in touch:  
- **Telegram**: [@koshurboii](https://t.me/koshurboii)
- **Instagram**: [@koshurboii](https://instagram.com/koshurboii)  
### YouTube
- **YouTube**: [@koshurboii](https://www.youtube.com/@koshurboii?sub_confirmation=1)

