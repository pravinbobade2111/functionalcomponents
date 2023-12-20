// App.js
import React from 'react';
import ExpenseItem from './ExpenseItem';

const App = () => {
  const expenses = [
    { title: 'Food', amount: 'Rs 10', locationOfExpenditure: 'Grocery Store' },
    { title: 'Petrol', amount: 'Rs 100', locationOfExpenditure: 'Gas Station' },
    { title: 'Movies', amount: 'Rs 200', locationOfExpenditure: 'Cinema' },
    // Add more expenses as needed
  ];

  return (
    <div>
      <h1>Expense Items</h1>
      {expenses.map((expense, index) => (
        <ExpenseItem
          key={index}
          title={expense.title}
          amount={expense.amount}
          locationOfExpenditure={expense.locationOfExpenditure}
        />
      ))}
    </div>
  );
};

export default App;
