![](https://venturebeat.com/wp-content/uploads/2018/02/google-flutter-logo.png?fit=578%2C289&strip=all)

***

## Plan
1. Introduction
2. Dart
3. World is Widget
4. Pro / Cons
5. Flutter web
6. Ressources

***

## Introduction

- 60 fps
- Hotreload
- Cross-plateforms

***

## Dart
![](https://dart.dev/assets/shared/dart-logo-for-shares.png?2&1)
Développé en 2011 par **Google**, pour remplacer le Javascript. Peut être compilé en **JS**.

- Typé
- Meilleure sécurité
- Meilleures performances

### Exemple 
Syntax proche du typescript :
```typescript
/* Typescript */
class Segement {
	links: number = 4

	public toString() : string {
		return `I have ${this.links} links.` 
	} 
}
```

```dart
/* Dart */
class Segment {
	int links = 4;

	toString() => "I have $links links"
}
```
***

## World is Widget

En Flutter, tout ce qui relève de l'UI est un *Widget*.

```dart
class MyWidget extends StatelessWidget {
	@override
	Widget build(BuildContext context) { ... }
}
```

### Stateless Widget
Un widget sans intéraction de l'utilisateur. Il ne fait que rendre les informations.

### Stateful Widget
Un widget qui permet des intéractions avec son *state* interne

***

## World is Widget > Librairies

- [Core widgets](https://flutter.dev/docs/development/ui/widgets)
- [Material](https://flutter.dev/docs/development/ui/widgets/material)
- [Cupertuino](https://flutter.dev/docs/development/ui/widgets/cupertino)

***

## Pro / Cons

\+ 60fps : la fluidité avant tout

\- Nouveau :  tout n'existe pas encore, tout n'est pas parfait...
\- Google : support iOS un peu moins bien

***

## Flutter web

AngularJS -> Angular -> [AngularDart](https://angulardart.dev/guide/setup) -?> Flutter web ?

***

## Ressources

- [Dart Dev](https://dart.dev/)
- [Dart Packages](https://pub.dev/)
- [Flutter Dev](https://flutter.dev/)
- [Flutter Youtube Channel](https://www.youtube.com/watch?v=b_sQ9bMltGU&list=PLjxrf2q8roU23XGwz3Km7sQZFTdB996iG) pour découvrir en moins de 60 secondes l'utilisation d'un widget
