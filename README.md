# AppGrupo8
int quitar_sede (FILE *myfile,char *filename){
  char sede;
  int opcion;
  printf("Nombre de la sede que desea eliminar: \n");
          scanf("%s",&sede);
  printf("La sede %s tiene libros asociados por lo que no se puede eliminar. Si deseas eliminar la sede debes borrar sus los libros asociados\n",&sede);
  printf("¿Quieres volver al paso 1? (si=1, no =2): \n");
  scanf("%i",&opcion);
  switch(opcion){
    case 1:
        opcion1(myfile,filename);
    case 2:
        break;
    default:
        printf("Ups, esa opcion no esta, intenta con otra\n");
            quitar_sede(myfile,filename);
    
  }
    
  return 0;
}

int quitar_seccion (FILE *myfile,char *filename){
  char seccion;
  int opcion;
  printf("Nombre de la seccion que desea eliminar: \n");
  scanf("%s",&seccion);
  printf("La seccion %s tiene libros asociados por lo que no se puede eliminar. Si deseas eliminar la seccion debes borrar sus los libros asociados\n",&seccion);
  printf("¿Quieres volver al paso 1? (Ingresa 1 para si y 2 para no: \n");
  scanf("%i",&opcion);
  switch(opcion){
    case 1:
        opcion1(myfile,filename);
    case 2:
        break;
    default:
        printf("Ups, esa opcion no esta, intenta con otra\n");
            quitar_seccion(myfile,filename);
    
  }
    
  return 0;
}

int quitar_piso (FILE *myfile,char *filename){
  int piso;
  int opcion;
  printf("Ingrese el piso que desea eliminar: \n");
  scanf("%d",&piso);
  printf("El piso %c tiene libros asociados por lo que no se puede eliminar. Si deseas eliminar este piso debes borrar sus los libros asociados\n",piso);
  printf("¿Quieres volver al paso 1? (Ingresa 1 para si y 2 para no): \n");
  scanf("%i",&opcion);
  switch(opcion){
    case 1:
        opcion1(myfile,filename);
    case 2:
        break;
    default:
        printf("Ups, esa opcion no esta, intenta con otra\n");
            quitar_piso(myfile,filename);
    
  }
    
  return 0;
}
