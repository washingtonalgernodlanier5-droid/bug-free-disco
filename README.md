@Entity
@Table(name = "users")
public class User {

    @Id
    @GeneratedValue(strategy =
        GenerationType.IDENTITY)

    private Long id;

    private String username;

    private String email;

    private String password;

    private String role;

    private boolean active = true;

    private boolean walletFrozen = false;

    private double totalBalance;

    private double totalProfit;
}
