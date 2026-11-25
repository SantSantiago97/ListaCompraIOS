# Lista de la Compra Inteligente (iOS WKWebView)

Contenedor iOS para cargar la aplicación web interactiva (`index.html`) con todo el catálogo, cálculo en tiempo real, edición de precios, modo eliminar y deshacer.

## Estructura incluida
- `www/index.html`: Aplicación web completa.
- `ListaCompraApp/ListaCompraApp.swift`: Punto de entrada de la app en SwiftUI.
- `ListaCompraApp/ContentView.swift`: Contenedor `WKWebView` a pantalla completa.

## Compilación y firma (.ipa)
- **En macOS con Xcode:** Crea un proyecto *iOS App* (SwiftUI), añade `ContentView.swift` y `ListaCompraApp.swift`, y usa *Product -> Archive -> Distribute App* para exportar el `.ipa`.
- **Sideloading / herramientas de firma:** Empaqueta el binario `arm64` firmado dentro de `Payload/ListaCompra.app/` y comprímelo en `.zip` renombrado a `.ipa` para instalarlo en tu iPhone.
