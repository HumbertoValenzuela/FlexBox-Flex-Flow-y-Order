# FlexBox-Flex-Flow-y-Order
### Flexbox uso de Order y order en ResponsiveDesign

*006 Flex Flow y Order
 *       Order: sirve para dar orden de mostrar un elemento. Util además para los Responsives Design media querys. 
 *       .elemento-flex:nth-child(1) pseudoclase para poder seleccionar un hijo
 *       Para que se muestre primero order: -1;
 *       Order no tiene ingerencia en html
 *       Uso de ResponsivesDesign usando Order
 
 *  para el escritorio el Order será 3 1 2 y para Tablet será 3 2 1 
```javascript
.elemento-flexOrder:nth-child(1) {
    background-color: #e72e21;
    order: 3;
}

.elemento-flexOrder:nth-child(2) {
    background-color: #8E24AA;
    order: 2;
}

.elemento-flexOrder:nth-child(3) {
    background-color: #3F51B5;
    order: 1;
}

@media screen and (min-width: 768px) {
    .elemento-flexOrder:nth-child(3) {
        background-color: #3F51B5;
        order: -1;/* para que se muestre primero*/
    }
    .elemento-flexOrder:nth-child(2) {
        background-color: #8E24AA;
        order: 3;
    }

}
```
