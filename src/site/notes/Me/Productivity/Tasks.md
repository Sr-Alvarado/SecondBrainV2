---
{"dg-publish":true,"permalink":"/me/productivity/tasks/","created":"2024-01-28T18:44","updated":"2024-07-05T17:14"}
---

## Gráfico de Goals vs Tareas
```mermaid
flowchart LR
   Goal3 & P1 & B1 --> P1.1 --> P1.1.1
   I1 --> I1.1
   C1 --> C1.1 --> C1.1.1 & C1.1.2
   C2 --> C2.1 --> C2.1.1

   subgraph Goal1 [Business]
      direction LR
   
      B1["`Sistema acuaponico domotico`"]
   end
   
      subgraph Goal2 [Code]
      direction LR
      
      P1["`Aprender lógica de programación`"]
      P1.1["`Hacer el curso Python 30 días`"]
      P1.1.1["`Terminar los ejercicios del [[Day 3 - Operadores]]`"] 
   end

   subgraph Goal3 [Aprender Inglés]
      direction LR
      
      I1["`Aprender vocabulario`"]
      I1.1["`Restaurar racha Anki`"]
   end

   subgraph Goal [Community]
      direction LR

      C1["`Mi propia organización`"]
      C1.1["`Proyecto festival Juvenil`"]
      C1.1.1["`Crear [[Plan base para festival]] Juvenil`"]
      C1.1.2["`Buscar alianzas para finaciar la actividad`"]
      C2["`Aprender de otras organizaciones`"]
      C2.1["`Apoyar en el proyecto de Red IQ`"]
      C2.1.1["`Explicar a Red IQ que no soy de ORCAA`"]
   end
```

## Legend
### Tags
🔥 : cosas que solo se hacen una vez, se define en el tiempo
🚀: acciones que se van a repetir en el tiempo, se coloca en una rutina
🛒: Que se tiene que comprar
### Priority
🔺 : Que se debe hacer **hoy** 
⏫ : Que se debe hacer **mañana o pasado mañana**
🔼 : Que se debe hacer **esta semana**
Todo lo demás no tiene prioridad
[[Me/Productivity/My be goals\|My be goals]]