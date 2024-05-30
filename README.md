# Ninox-Modal-Plugin

## German

## Übersicht
Dieses Plugin ermöglicht es Nutzern, Modals und Toasts dynamisch einblenden zu lassen.

## Funktionen

### showToast
Zeigt eine Toast-Benachrichtigung an.

**Verwendung:**

```javascript
showToast({
    uniqueId: 'einzigartigeID',
    caption: 'Benachrichtigung',
    message: 'Dies ist eine Beispielnachricht.',
    time: 5000,
    minWidth: '300px',
    maxWidth: '600px',
    padding: '15px',
    alignX: 'right',
    alignY: 'bottom',
    animation: {
        in: 'fadeIn',
        out: 'fadeOut',
        timeIn: 500,
        timeOut: 500,
        directionIn: 'bottom',
        directionOut: 'bottom'
    },
    backgroundColor: "#fff",
    borderRadius: "8px",
    fontColor: "#000",
    closeButton: true,
    closeButtonBackgroundColor: "#ff5f57",
    closeButtonFontColor: "#000",
    styles: {
        header: { fontSize: '18px', color: '#333' },
        message: { fontSize: '14px', color: '#555' },
        colorBar: { width: '4px', backgroundColor: '#007bff', borderRadius: '8px' }
    },
    showProgressBar: false,
    progressBarPosition: 'bottom',
    progressBarColor: '#007bff'
});
```

### showModal
Zeigt ein modales Pop-up an.

**Verwendung:**

```javascript
showModal({
    uniqueId: 'einzigartigeID',
    caption: 'Benachrichtigung',
    message: 'Dies ist eine Beispielnachricht.',
    time: 5000,
    minWidth: '300px',
    maxWidth: '600px',
    padding: '15px',
    alignX: 'center',
    alignY: 'center',
    animationIn: 'fadeIn',
    animationOut: 'fadeOut',
    animationDirectionIn: 'bottom',
    animationDirectionOut: 'bottom',
    animationTimeIn: 500,
    animationTimeOut: 500,
    backgroundColor: '#323232',
    borderRadius: '8px',
    fontColor: 'white',
    closeButton: true,
    closeButtonBackgroundColor: '#ff5f57',
    closeButtonFontColor: 'white',
    styles: {
        header: { fontSize: '24px', color: 'rgb(100, 100, 100)' },
        message: { fontSize: '12px', color: 'rgb(100, 100, 100)' }
    },
    showProgressBar: false,
    progressBarPosition: 'bottom',
    progressBarColor: '#007bff'
});
```

## JSON-Objekt für das Styling
Die Styling-Optionen können über das styles-Objekt angepasst werden:

- header: Stile für den Header-Bereich
  - fontSize: Schriftgröße des Headers
  - color: Schriftfarbe des Headers
- message: Stile für den Nachrichtenbereich
  - fontSize: Schriftgröße der Nachricht
  - color: Schriftfarbe der Nachricht
- colorBar: Stile für die Farbleiste (Toast)
  - width: Breite der Farbleiste
  - backgroundColor: Hintergrundfarbe der Farbleiste
  - borderRadius: Eckenradius der Farbleiste

Beispiel:

```javascript
styles: {
    header: { fontSize: '18px', color: '#333' },
    message: { fontSize: '14px', color: '#555' },
    colorBar: { width: '4px', backgroundColor: '#007bff', borderRadius: '8px' }
}
````

## English

## Overview
This plugin allows users to dynamically display modals and toasts.

## Functions
### showToast
Displays a toast notification.

***Usage:***

```javascript
showToast({
    uniqueId: 'uniqueID',
    caption: 'Notification',
    message: 'This is a sample message.',
    time: 5000,
    minWidth: '300px',
    maxWidth: '600px',
    padding: '15px',
    alignX: 'right',
    alignY: 'bottom',
    animation: {
        in: 'fadeIn',
        out: 'fadeOut',
        timeIn: 500,
        timeOut: 500,
        directionIn: 'bottom',
        directionOut: 'bottom'
    },
    backgroundColor: "#fff",
    borderRadius: "8px",
    fontColor: "#000",
    closeButton: true,
    closeButtonBackgroundColor: "#ff5f57",
    closeButtonFontColor: "#000",
    styles: {
        header: { fontSize: '18px', color: '#333' },
        message: { fontSize: '14px', color: '#555' },
        colorBar: { width: '4px', backgroundColor: '#007bff', borderRadius: '8px' }
    },
    showProgressBar: false,
    progressBarPosition: 'bottom',
    progressBarColor: '#007bff'
});
```

## showModal
Displays a modal pop-up.

***Usage:***

```javascript
showModal({
    uniqueId: 'uniqueID',
    caption: 'Notification',
    message: 'This is a sample message.',
    time: 5000,
    minWidth: '300px',
    maxWidth: '600px',
    padding: '15px',
    alignX: 'center',
    alignY: 'center',
    animationIn: 'fadeIn',
    animationOut: 'fadeOut',
    animationDirectionIn: 'bottom',
    animationDirectionOut: 'bottom',
    animationTimeIn: 500,
    animationTimeOut: 500,
    backgroundColor: '#323232',
    borderRadius: '8px',
    fontColor: 'white',
    closeButton: true,
    closeButtonBackgroundColor: '#ff5f57',
    closeButtonFontColor: 'white',
    styles: {
        header: { fontSize: '24px', color: 'rgb(100, 100, 100)' },
        message: { fontSize: '12px', color: 'rgb(100, 100, 100)' }
    },
    showProgressBar: false,
    progressBarPosition: 'bottom',
    progressBarColor: '#007bff'
});
```

### Closing Toast and Modal
To manually close a toast or modal, use the following functions:

```javascript
closeToast(document.getElementById('uniqueID'));
closeModal(document.getElementById('uniqueID'));
```

## JSON Object for Styling
Styling options can be customized using the styles object:

- header: Styles for the header section
  - fontSize: Font size of the header
  - color: Font color of the header
- message: Styles for the message section
  - fontSize: Font size of the message
  - color: Font color of the message
- colorBar: Styles for the color bar (toast)
  - width: Width of the color bar
  - backgroundColor: Background color of the color bar
  - borderRadius: Corner radius of the color bar
Example:

```javascript
styles: {
    header: { fontSize: '18px', color: '#333' },
    message: { fontSize: '14px', color: '#555' },
    colorBar: { width: '4px', backgroundColor: '#007bff', borderRadius: '8px' }
}
```
