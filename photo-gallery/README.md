# Projet-ionic-vue-demo
 
npm install -g @ionic/cli@latest native-run cordova-res

# Create an App​
ionic start photo-gallery tabs --type vue --capacitor

cd photo-gallery

npm install @capacitor/camera @capacitor/storage @capacitor/filesystem

# PWA Elements​
npm install @ionic/pwa-elements

Next, import @ionic/pwa-elements by editing src/main.ts.
// Above the createApp() line
import { defineCustomElements } from '@ionic/pwa-elements/loader';

// Call the element loader after the platform has been bootstrapped
defineCustomElements(window);

# Run the App​
ionic serve