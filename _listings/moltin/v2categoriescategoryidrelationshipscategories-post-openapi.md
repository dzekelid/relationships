---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Create Parent Category Relationship
  description: Using this endpoint you can create a relationship between a category
    and a parent category. When returning the category tree, you will see this relationship
    in place.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/products/{productID}/relationships/variations:
    put:
      summary: Update Product <=> Variations Relationships
      description: '`Product Variation`''s specified in the payload willbe related
        to the `Product` any relatiosnhips to `Product Variation`''s **NOT** specified
        in payload will be removed.'
      operationId: V2ProductsRelationshipsVariationsByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipsvariations-put
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variations
      - Relationships
    post:
      summary: Create Product <=> Variations Relationships
      description: Here you can add and remove `Product Variation`'s to a product.
        `Product Variation`'s specified in the payload willbe related to the product.
      operationId: V2ProductsRelationshipsVariationsByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipsvariations-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variations
      - Relationships
    delete:
      summary: Delete Product <=> Variations Relationships
      description: Here you can add and remove `Product Variation`'s to a product.
        Only relationships to `Product Variation`'s specified in the payload will
        be removed.
      operationId: V2ProductsRelationshipsVariationsByProductIDDelete
      x-api-path-slug: v2productsproductidrelationshipsvariations-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variations
      - Relationships
  /v2/products/{productID}/relationships/files:
    put:
      summary: Update Products <=> Files Relationships
      description: '`File`''s specified in the payload willbe related to the product
        any relatiosnhips to `File`''s **NOT** specified in payload will be removed.'
      operationId: V2ProductsRelationshipsFilesByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipsfiles-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Files
      - Relationships
    post:
      summary: Create Products <=> Files Relationships
      description: Here you can add `File`'s to a product. `File`'s specified in the
        payload willbe related to the product.
      operationId: V2ProductsRelationshipsFilesByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipsfiles-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Files
      - Relationships
    delete:
      summary: Delete Products <=> Files Relationship
      description: Here you can delete a relationship between a `Product` and `File`'s.
        Only relationships to `File`'s specified in the payload will be removed.
      operationId: V2ProductsRelationshipsFilesByProductIDDelete
      x-api-path-slug: v2productsproductidrelationshipsfiles-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Files
      - Relationship
  /v2/collections/{collectionID}/relationships/collections:
    post:
      summary: Create Collection Relationships
      description: Create collection relationships.
      operationId: V2CollectionsRelationshipsCollectionsByCollectionIDPost
      x-api-path-slug: v2collectionscollectionidrelationshipscollections-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collection
      - Relationships
  /v2/categories/{categoryID}/relationships/children:
    put:
      summary: Update Child Category Relationships
      description: Update child category relationships.
      operationId: V2CategoriesRelationshipsChildrenByCategoryIDPut
      x-api-path-slug: v2categoriescategoryidrelationshipschildren-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Category
      - Relationships
    delete:
      summary: Delete Child Category Relationships
      description: Delete child category relationships.
      operationId: V2CategoriesRelationshipsChildrenByCategoryIDDelete
      x-api-path-slug: v2categoriescategoryidrelationshipschildren-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Category
      - Relationships
  /categories/{categoryID}/relationships/children:
    post:
      summary: Create Child Category Relationships
      description: Create child category relationships.
      operationId: CategoriesRelationshipsChildrenByCategoryIDPost
      x-api-path-slug: categoriescategoryidrelationshipschildren-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Category
      - Relationships
  /v2/products/{productID}/relationships/brands:
    put:
      summary: Update Product <=> Brands Relationships
      description: Here you can set relations `Brand`'s to a product. The result of
        this request will set relationships between product and the specified brnads
        in teh payload and remove any other relations the product had with brands.
      operationId: V2ProductsRelationshipsBrandsByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipsbrands-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Brandss
      - Relationships
    post:
      summary: Create Product <=> Brands Relationships
      description: Here you can add `Brand`'s to a product. The `Brand`'s found in
        the payload will be added to any other relationships to `Brand`'s present.
      operationId: V2ProductsRelationshipsBrandsByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipsbrands-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Brandss
      - Relationships
    delete:
      summary: Delete Products <=> Brands Relationships
      description: Here you can delete a relationship between a `Product` and `Brand`'s.
        Only those relationshops to `Brand`'s specified in the paylaod will be removed.
      operationId: V2ProductsRelationshipsBrandsByProductIDDelete2
      x-api-path-slug: v2productsproductidrelationshipsbrands-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Brands
      - Relationships
  /v2/products/{ProductID}relationships/brands:
    post:
      summary: Create Products <=> Main Image Relationships
      description: |-
        Here you can add a `Main Image` to a product. The `Main Image` will be a file and that file will be shown as the first image for the product it is related to.

        It's worth noting that you can only have 1 main image so unlike other relationships, you will be passing an object instead of an array in the body.

        In the Object, the type will be `main_image` and the ID will be the ID of the file you wish to make the main image for that product.
      operationId: V2ProductsRelationshipsBrandsByProductIDPost2
      x-api-path-slug: v2productsproductidrelationshipsbrands-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: ProductID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Main
      - Image
      - Relationships
    delete:
      summary: Delete Products <=> Main Image Relationships
      description: |-
        Here you can delete the `Main Image` from a product.

        In the Object payload, the type will be `main_image` and the ID will be the ID of the main image you wish to delete from that product.
      operationId: V2ProductsRelationshipsBrandsByProductIDDelete
      x-api-path-slug: v2productsproductidrelationshipsbrands-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: ProductID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Main
      - Image
      - Relationships
  /v2/products/{productID}/relationships/categories:
    put:
      summary: Update Product <=> Categories Relationships
      description: Here you can update `Categories` to a product. `Categories` specified
        in the payload willbe related to the product any relatiosnhips to `Categories`
        **NOT** specified in payload will be removed.
      operationId: V2ProductsRelationshipsCategoriesByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipscategories-put
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Categories
      - Relationships
    post:
      summary: Create Product <=> Categories Relationships
      description: Here you can add `Categories` to a product. `Categories` specified
        in the payload willbe related to the product.
      operationId: V2ProductsRelationshipsCategoriesByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipscategories-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Categories
      - Relationships
    delete:
      summary: Delete Product <=> Categories Relationships
      description: Here you can delete a relationship between a `Product` and `Category`.
        Only relationships to `Categories` specified in the payload will be removed.
      operationId: V2ProductsRelationshipsCategoriesByProductIDDelete
      x-api-path-slug: v2productsproductidrelationshipscategories-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Categories
      - Relationships
  /v2/products/{productID}/relationships/collections:
    put:
      summary: Update Products <=> Collections Relationships
      description: '`Collection`''s specified in the payload willbe related to the
        product any relatiosnhips to `Collection`''s **NOT** specified in payload
        will be removed.'
      operationId: V2ProductsRelationshipsCollectionsByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipscollections-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Collections
      - Relationships
    post:
      summary: Create Products <=> Collections Relationships
      description: Here you can add `Collection`'s to a product. `Collection`'s specified
        in the payload willbe related to the product.
      operationId: V2ProductsRelationshipsCollectionsByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipscollections-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Collections
      - Relationships
    delete:
      summary: Delete Products <=> Collections Relationships
      description: Here you can delete a relationship between a `Product` and `Collections`.
        Only relationships to `Collections` specified in the payload will be removed.
      operationId: V2ProductsRelationshipsCollectionsByProductIDDelete
      x-api-path-slug: v2productsproductidrelationshipscollections-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - Collections
      - Relationships
  /categories/{categoryID}/relationships/categories:
    delete:
      summary: Delete Category-Category Relationships
      description: Delete category-category relationships.
      operationId: CategoriesRelationshipsCategoriesByCategoryIDDelete
      x-api-path-slug: categoriescategoryidrelationshipscategories-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category-Category
      - Relationships
  /v2/collections/{collectionID}/relationships/children:
    post:
      summary: Create Child Collection Relationships
      description: Create child collection relationships.
      operationId: V2CollectionsRelationshipsChildrenByCollectionIDPost
      x-api-path-slug: v2collectionscollectionidrelationshipschildren-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Collection
      - Relationships
    put:
      summary: Update Child Collection Relationship
      description: Update child collection relationship.
      operationId: V2CollectionsRelationshipsChildrenByCollectionIDPut
      x-api-path-slug: v2collectionscollectionidrelationshipschildren-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Collection
      - Relationship
    delete:
      summary: Delete Child Collection Relationship
      description: Delete child collection relationship.
      operationId: V2CollectionsRelationshipsChildrenByCollectionIDDelete
      x-api-path-slug: v2collectionscollectionidrelationshipschildren-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Collection
      - Relationship
  /v2/brands/{brandID}/relationships/brands:
    post:
      summary: Create Brand Relationships
      description: Create brand relationships.
      operationId: V2BrandsRelationshipsBrandsByBrandIDPost
      x-api-path-slug: v2brandsbrandidrelationshipsbrands-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Brands
      - Relationships
  /v2/brands/{brandID}/relationships/parent:
    put:
      summary: Update Parent Brand Relationship
      description: Update parent brand relationship.
      operationId: V2BrandsRelationshipsParentByBrandIDPut
      x-api-path-slug: v2brandsbrandidrelationshipsparent-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Brands
      - Relationship
    post:
      summary: Create Parent Brand Relationship
      description: Create parent brand relationship.
      operationId: V2BrandsRelationshipsParentByBrandIDPost
      x-api-path-slug: v2brandsbrandidrelationshipsparent-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Brands
      - Relationship
    delete:
      summary: Delete Parent Brand Relationship
      description: Delete parent brand relationship.
      operationId: V2BrandsRelationshipsParentByBrandIDDelete
      x-api-path-slug: v2brandsbrandidrelationshipsparent-delete
      parameters:
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Brands
      - Relationship
  /v2/brands/{brandID}/relationships/children:
    put:
      summary: Update Child Brand Relationship
      description: Update child brand relationship.
      operationId: V2BrandsRelationshipsChildrenByBrandIDPut
      x-api-path-slug: v2brandsbrandidrelationshipschildren-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Brands
      - Relationship
    post:
      summary: Create Child Brand Relationship
      description: Create child brand relationship.
      operationId: V2BrandsRelationshipsChildrenByBrandIDPost
      x-api-path-slug: v2brandsbrandidrelationshipschildren-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Brands
      - Relationship
    delete:
      summary: Update Child Brand Relationship Copy
      description: Update child brand relationship copy.
      operationId: V2BrandsRelationshipsChildrenByBrandIDDelete
      x-api-path-slug: v2brandsbrandidrelationshipschildren-delete
      parameters:
      - in: path
        name: brandID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Brands
      - Relationship
      - Copy
  /v2/collections/{collectionID}/relationships/parent:
    put:
      summary: Update Parent Collection Relationship
      description: Update parent collection relationship.
      operationId: V2CollectionsRelationshipsParentByCollectionIDPut
      x-api-path-slug: v2collectionscollectionidrelationshipsparent-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Collection
      - Relationship
    post:
      summary: Create Parent Collection Relationship
      description: Create parent collection relationship.
      operationId: V2CollectionsRelationshipsParentByCollectionIDPost
      x-api-path-slug: v2collectionscollectionidrelationshipsparent-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Collection
      - Relationship
    delete:
      summary: Delete Parent Collection Relationship
      description: Delete parent collection relationship.
      operationId: V2CollectionsRelationshipsParentByCollectionIDDelete
      x-api-path-slug: v2collectionscollectionidrelationshipsparent-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: collectionID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Collection
      - Relationship
  /v2/categories/{categoryID}/relationships/categories:
    post:
      summary: Create Parent Category Relationship
      description: Using this endpoint you can create a relationship between a category
        and a parent category. When returning the category tree, you will see this
        relationship in place.
      operationId: V2CategoriesRelationshipsCategoriesByCategoryIDPost
      x-api-path-slug: v2categoriescategoryidrelationshipscategories-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Category
      - Relationship
  /v2/flows/{flowSlug}/entries/{ENTRY_ID}/relationships/{flowSlug}:
    put:
      summary: Update Entry Relationship(s)
      description: Update entry relationship(s).
      operationId: V2FlowsEntriesRelationshipsFlowSlugByFlowSlugAndENTRYIDPut
      x-api-path-slug: v2flowsflowslugentriesentry-idrelationshipsflowslug-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: ENTRY_ID
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Entry
      - Relationship(s)
    delete:
      summary: Delete Entry Relationship(s)
      description: Delete entry relationship(s).
      operationId: V2FlowsEntriesRelationshipsFlowSlugByFlowSlugAndENTRYIDDelete
      x-api-path-slug: v2flowsflowslugentriesentry-idrelationshipsflowslug-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: ENTRY_ID
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Entry
      - Relationship(s)
  /v2/flows/{flowSlug}/entries/{entryID}/relationships/{fieldSlug}:
    post:
      summary: Create Entry Relationship(s)
      description: Create entry relationship(s).
      operationId: V2FlowsEntriesRelationshipsFieldSlugByFlowSlugAndEntryIDPost
      x-api-path-slug: v2flowsflowslugentriesentryidrelationshipsfieldslug-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: entryID
      - in: path
        name: fieldSlug
      - in: path
        name: flowSlug
      responses:
        200:
          description: Successful response
      tags:
      - Entry
      - Relationship(s)
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---