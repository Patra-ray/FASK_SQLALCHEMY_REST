# FASK_SQLALCHEMY_REST
https://www.youtube.com/watch?v=PTZiDnuC86g

Due to changes in Marshmallow from version 2 to version 3, the following were changed:

# schema no longer need strict=True parameter 

was
product_schema = ProductSchema(strict=True )
products_schema = ProductSchema(many=True), strict=True)

now 
product_schema = ProductSchema()
products_schema = ProductSchema(many=True)


# type error of List

was
jsonify(result.data)

now
jsonify(result)
