# controle.continu
import 'package:flutter/material.dart';

void main() {
  runApp(
    Myapp(),
  );
}

class Myapp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        backgroundColor: Colors.tealAccent,
        body: SafeArea(
          child: Column(
            mainAxisAlignment: MainAxisAlignment.center ,
            children: <Widget>[
              CircleAvatar(
                radius: 50.0,
                backgroundImage: AssetImage('image/gon.jpg'),
              ),
              Text(
                'Kelkoul Tasnime',
                style: TextStyle(
                  fontFamily: 'Source sans pro',
                  fontSize: 15.0,
                  color: Colors.black,
                  letterSpacing: 2.5,
                  fontWeight: FontWeight.bold,
                ),
              ),
              Text(
                'Ingenieur',
                style: TextStyle(
                  fontFamily: 'Pacifico',
                  fontSize: 40.0,
                  color: Colors.white,
                  fontWeight: FontWeight.bold,
                ),
              ),
              Container(
                color: Colors.white,
                margin: EdgeInsets.symmetric(vertical: 10.0, horizontal: 25.0),
                padding: EdgeInsets.all(10.0),
                child: Row(
                  children: <Widget>[
                    Icon(
                      Icons.call,
                      size: 20.0,
                      color: Colors.teal.shade900,
                    ),
                    SizedBox(
                      width: 10.0,
                    ),
                    Text(
                      "07 58 92 65 76",
                      style: TextStyle(
                          color: Colors.teal.shade900,
                          fontFamily: 'Source sans pro'),
                    )
                  ],
                ),
              ),
              Container(
                color: Colors.white,
                margin: EdgeInsets.symmetric(vertical: 10.0, horizontal: 25.0),
                padding: EdgeInsets.all(10.0),
                child: Row(
                  children: <Widget>[
                    Icon(
                      Icons.android,
                      size: 20.0,
                      color: Colors.teal.shade900,
                    ),
                    SizedBox(
                      width: 10.0,
                    ),
                    Text(
                      "tasnime.klk@gmail.com",
                      style: TextStyle(
                          color: Colors.teal.shade900,
                          fontFamily: 'Source sans pro'),
                    )
                  ],
                ),
              ),
            ],
          ),
        ),
      ),
    );
  }
}
