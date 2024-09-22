# Try
const formData = {
  username: 'user123',
  password: 'pass',
  email: 'user@example.com',
};

const validationRules = {
  username: { required: true, minLength: 5 },
  password: { required: true, minLength: 8 },
  email: { required: true, email: true },
};

const result = validateForm(formData, validationRules);
console.log(result);
// Output: { valid: false, errors: { password: 'Password must be at least 8 characters.' } }
