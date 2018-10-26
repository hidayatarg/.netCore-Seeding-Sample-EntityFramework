# .netCore-Seeding-SampleData-EntityFramework
Place in the Context.cs 

```csharp
protected override void OnModelCreating(ModelBuilder modelBuilder)
{
    modelBuilder.Entity<Group>()
      .HasData(
        new Group() {Id = 1, Name = "Super Admin", Description = "Super Admin" },
        new Group() { Id = 2, Name = "Admin", Description = "Admin"},
        new Group() { Id = 3, Name = "Normal", Description = "Normal"} 
     );
}
```
