public class BankAccount {
    private String accountHolderName;
    private String accountNumber;
    private double balance;

    public BankAccount(String accountHolderName, String accountNumber, double balance) {
        this.accountHolderName = accountHolderName;
        this.accountNumber = accountNumber;
        this.balance = balance;
    }

    public void deposit(double amount) {
        if (amount > 0) {
            balance += amount;
            System.out.println("Deposit of " + amount + "rs successful. New balance: " + balance+"rs");
        } else {
            System.out.println("Invalid deposit amount. Please enter a positive amount.");
        }
    }

    public void withdraw(double amount) {
        if (amount > 0) {
            if (amount <= balance) {
                balance -= amount;
                System.out.println("Withdrawal of " + amount + "rs successful. New balance: " + balance+"rs");
            } else {
                System.out.println("Insufficient funds. Withdrawal unsuccessful.");
            }
        } else {
            System.out.println("Invalid withdrawal amount. Please enter a positive amount.");
        }
    }
    public void displayBalance() {
        System.out.println("Account Holder: " + accountHolderName);
        System.out.println("Account Number: " + accountNumber);
        System.out.println("Current Balance: " + balance+"rs");
    }
    public static void main(String[] args) {
        BankAccount account = new BankAccount("mukesh", "9999999999", 1000);
        account.deposit(500);
        account.withdraw(200);
        account.displayBalance();
    }
}
