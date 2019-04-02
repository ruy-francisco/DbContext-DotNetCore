* `DbContext` "MUST" to have an instance of `DbContextOptions`.
* `DbContextOptions` carries config information such as:
..* The database provider to be used
..* Here we use `Microsoft.EntityFrameworkCore` namespace
..* The `DbContextOptions` can be supplied by overriding the `OnConfiguring` method or externally via a constructor argument. It's necessary to be carefull because `OnConfiguring` executes after constructor and can override the constructor argumente behavior.
* Any connection string or identifier of the database instance
