import 'package:flutter/material.dart';
void main() => runApp(MyApp());
class MyApp extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return MaterialApp(
 home: GridViewDemo(),
 );
 }
}
class GridViewDemo extends StatelessWidget {
 @override
 Widget build(BuildContext context) {
 return Scaffold(
 appBar: AppBar(title: Text('GridView Example')),
 body: GridView.count(
 crossAxisCount: 3, // Number of columns
 padding: EdgeInsets.all(10),
 children: <Widget>[
 Container(
 color: Colors.red,
 child: Center(child: Text('Item 1')),
 ),
 Container(
 color: Colors.green,
 child: Center(child: Text('Item 2')),
 ),
 Container(
 color: Colors.blue,
 child: Center(child: Text('Item 3')),
 ),
 Container(
 color: Colors.orange,
 child: Center(child: Text('Item 4')),
 ),
 Container(
 color: Colors.purple,
 child: Center(child: Text('Item 5')),
 ),
 Container(
 color: Colors.yellow,
 child: Center(child: Text('Item 6')),
 ),
 ],
 ),
 );
 }
}
