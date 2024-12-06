## Windows PowerShell ki security setting ko badalta hai
 ka kam yeh hai ke yeh Windows PowerShell ki security setting ko badalta hai. 

Jab aap PowerShell mein scripts run karte hain, to kuch scripts ko run hone se rok diya jata hai agar unhe trusted source se nahi liya gaya ho. `RemoteSigned` ka matlab hai ke aap apni local machine pe likhi hui scripts ko run kar sakte hain, lekin internet se download ki hui scripts ko run karne ke liye unka signature hona zaroori hoga (yaani wo trusted source se honi chahiye).

Is command ka istemal aap ne is liye kiya tha taake `npx` jaise tools ko apne system par scripts run karne ki permission mil sake, taake aap Next.js project create kar sakein.

```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

A press and ente to all done 
