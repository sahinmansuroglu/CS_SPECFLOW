## AutoFixture ##

otomatik test verisi oluşturur.

```csharp
var person = new Fixture().Build<User>()
                .With(x => x.EMail, "sahin@meb.gov.tr")
                .Create(); ;
            Console.WriteLine($"The user {person.Name} has email {person.EMail} and his address {person.Address} and his phone number {person.Phone}");
private string GetRandomDomain() => new Fixture().Create<MailAddress>().Host;        
public record User
    {

        public string Name { get; set; }
        public string EMail { get; set; }
        public string Address { get; set; }
        public int Phone { get; set; }

    }
```
