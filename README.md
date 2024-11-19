# Aplicacion Yes Not Flutter
-----

## DESCRIPCION:

Proyecto de Clase para la Unidad 2 de la Asignatura de Desarrollo Móvil Integral (DMI) impartida
por el M.T.I Marco A. Ramírez Hernández

## HISTORIAL DE PRÁCTICAS:
|No. |Nombre|Potenciador|Estatus|
|--|--|--|--|
|22|Implementacion de la UI para la aplicación|10|Activa|
|21|Implementación de la funcionalidad de la aplicacion|10|Activa|

## LISTA DE HERRAMIENTAS
![DART](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)

## AUTOR
Elaborado por: Juan Manuel Cruz Ortiz [@jjuancoo](https://github.com/jjuancoo)

![Captura de pantalla 2024-11-13 223529](https://github.com/user-attachments/assets/ee266eb7-9f86-45c5-9196-5933efac566b)
![LOGO UNIVERSIDAD 1](https://github.com/user-attachments/assets/f0c4f5fc-173d-4ee0-b9ee-023ca1fe3ea9)

|No. |Nombre|Estudiante|Carrera|
|--|--|
|Nombre del estudiante|Juan Manuel Cruz Ortiz|Carrera|Ingenieria en Desarrollo de Software|

|No. |Nombre|Materia|Carrera|
|--|--|--|--|
|00|Juan Manuel Cruz Ortiz|Desarrollo Movil Integrador|Ingenieria en Desarrollo y Gestion de Software|

## PRACTICA 22 y 23: Definir la funcionalidad e UI para la aplicación de Yes Not
### Objetivo 

Desarrollar una aplicación en Flutter que simule una respuesta con caracteristicas visuales de un chat de alguna aplicacion de mensajeria.

### Descripción:

Este proyecto es una aplicación móvil en Flutter que incluye chat interactivo simulando la respuesta de otra persona con una UI de un app de mensajeria basado en material 3, nosotros preguntamos y el chat no devuelve una respuesta acompañado de una imagen simulando un "meme".

    Para continuar la conversación la pregunta debe de terminar con un ?.

Esta aplicacion contiene la respuesta de una api para mostrar las imagenes.

## Codigo y Estructura de las carpetas

### main.dart
    import 'package:flutter/material.dart';
    import 'package:provider/provider.dart';
    
    import 'package:yes_no_app/config/theme/app_theme.dart';
    import 'package:yes_no_app/presentation/providers/chat_provider.dart';
    import 'package:yes_no_app/presentation/screens/chat/chat_screen.dart';
    
    void main() => runApp(const MyApp());
    
    class MyApp extends StatelessWidget {
      const MyApp({super.key});
    
      @override
      Widget build(BuildContext context) {
        return MultiProvider(
          providers: [
            ChangeNotifierProvider(create: (_) => ChatProvider() )
          ],
          child: MaterialApp(
            title: 'Yes No App 210373',
            debugShowCheckedModeBanner: false,
            theme: AppTheme( selectedColor: 0 ).theme(),
            home: const ChatScreen()
          ),
        );
      }
    }


### Estructura de las carpetas
![Captura de pantalla 2024-11-19 094648](https://github.com/user-attachments/assets/ef568897-4166-4b80-b34e-fbc7c8acfe58)
Para consultar el codigo fuente, ve en este repositorio

### Imagenes de la app
![Imagen de WhatsApp 2024-11-19 a las 09 48 37_7c6bc588](https://github.com/user-attachments/assets/b1b0d703-1022-4d7f-8ead-ba8b457c2991)
