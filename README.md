# Comandos de Insercción y Consultas 

## Inserciones 🚀

 INSERT INTO paises(nombre) VALUES ('Colombia');

INSERT INTO ciudades(nombre,pais_id) VALUES ('Cucuta','1');

INSERT INTO sucursales(nombre,direccion,ciudad_id) VALUES ('Nueva Avenida','Av 12 #13AD-43 Pueblo Nuevo','1');

INSERT INTO clientes(nombre,email,direccion,telefono) VALUES ('Wilmer Gelves','wilgelgar98@gmail.com','Calle 5 #12-42 Campo dos','3103287849');

INSERT INTO paquetes(numero_seguimiento,peso,dimensiones,contenido,valor_declarado,tipo_servicio,estado) VALUES ('12345','12.5','4 de ancho x 1.5 de largo','Contine un epejo','200','nacional','por enviar');

INSERT INTO conductores(nombre,telefono) VALUES ('Carlos Enrique Perez','3103234242');

INSERT INTO rutas(descripcion,sucursal_id) VALUES ('Ruta manizales','1');

 INSERT INTO envios(cliente_id,paquete_id,conductor_id,fecha_de_envio,destino,ruta_id,sucursal_id) VALUES ('1','1','1','2024-10-29','Manizales','1','1');
ALTER TABLE envios
CHANGE COLUMN fecha_envio fecha_de_envio DATE NOT NULL;

ALTER TABLE envios CHANGE COLUMN fecha_envio fecha_de_envio DATE NOT NULL;

INSERT INTO envios(cliente_id,paquete_id,conductor_id,fecha_de_envio,destino,ruta_id,sucursal_id) VALUES ('1','1','1','2024-10-29','Manizales','1','1');

INSERT INTO auxiliares(nombre,telefono) VALUES ('Julio Garcia','310334234');

INSERT INTO  ruta_auxiliares(ruta_id,auxiliar_id) VALUES ('1','1');

ALTER TABLE seguimiento
CHANGE COLUMN fecha_hora fecha_hora DATE NOT NULL;

INSERT INTO seguimiento(paquete_id,ubicacion,fecha_hora,estado) VALUES ('1','Zona principal Manizales','2024-10-27','En camino');

