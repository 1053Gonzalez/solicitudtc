# solicitudtc
El proyecto consiste en implementar Restful a la aplicacion creada en el anterior video: https://studio.youtube.com/video/nDbWONOF96M/edit  para esta implementacion estamos usando Java 17 con SpringBoo7 3.2,  Maven y lombok y MySQL


## crear BD

CREATE DATABASE `jsf_jpa_centaurosbank` /*!40100 DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_general_ci */;

## Crear Tabla

CREATE TABLE `solicitudtc` (
  `id_solicitud` int(11) NOT NULL AUTO_INCREMENT,
  `autoriza_tratamiento_datos` bit(1) NOT NULL,
  `cedula_ciudadania` varchar(20) NOT NULL,
  `correo_electronico` varchar(100) NOT NULL,
  `direccion` varchar(200) NOT NULL,
  `fecha_expedicion` date NOT NULL,
  `fecha_nacimiento` date NOT NULL,
  `nombres` varchar(255) NOT NULL,
  `numero_celular` varchar(20) NOT NULL,
  `primer_apellido` varchar(255) NOT NULL,
  `segundo_apellido` varchar(255) DEFAULT NULL,
  PRIMARY KEY (`id_solicitud`)
) ENGINE=InnoDB AUTO_INCREMENT=11 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

