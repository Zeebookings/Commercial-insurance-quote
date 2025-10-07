<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Business Insurance Quote Request</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Arial, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
        }
        
        .container {
            max-width: 800px;
            margin: 0 auto;
            background: white;
            border-radius: 12px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.1);
            overflow: hidden;
        }
        
        .header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 40px 30px;
            text-align: center;
        }
        
        .header h1 {
            font-size: 32px;
            margin-bottom: 10px;
        }
        
        .header p {
            font-size: 16px;
            opacity: 0.95;
        }
        
        .form-content {
            padding: 40px 30px;
        }
        
        .section {
            margin-bottom: 40px;
        }
        
        .section-title {
            font-size: 24px;
            color: #667eea;
            margin-bottom: 25px;
            padding-bottom: 10px;
            border-bottom: 3px solid #667eea;
        }
        
        .form-group {
            margin-bottom: 25px;
        }
        
        label {
            display: block;
            font-weight: 600;
            color: #333;
            margin-bottom: 8px;
            font-size: 15px;
        }
        
        .required {
            color: #e74c3c;
            margin-left: 3px;
        }
        
        input[type="text"],
        input[type="email"],
        input[type="tel"],
        input[type="date"],
        input[type="number"],
        select,
        textarea {
            width: 100%;
            padding: 12px 15px;
            border: 2px solid #e0e0e0;
            border-radius: 6px;
            font-size: 15px;
            transition: all 0.3s ease;
            font-family: inherit;
        }
        
        input:focus,
        select:focus,
        textarea:focus {
            outline: none;
            border-color: #667eea;
            box-shadow: 0 0 0 3px rgba(102, 126, 234, 0.1);
        }
        
        textarea {
            resize: vertical;
            min-height: 100px;
        }
        
        .checkbox-group,
        .radio-group {
            display: flex;
            flex-direction: column;
            gap: 10px;
        }
        
        .checkbox-item,
        .radio-item {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        input[type="checkbox"],
        input[type="radio"] {
            width: 20px;
            height: 20px;
            cursor: pointer;
        }
        
        input[type="file"] {
            padding: 10px;
            border: 2px dashed #667eea;
            border-radius: 6px;
            background: #f8f9ff;
            cursor: pointer;
        }
        
        input[type="file"]:hover {
            background: #f0f2ff;
        }
        
        .submit-btn {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 15px 40px;
            border: none;
            border-radius: 6px;
            font-size: 18px;
            font-weight: 600;
            cursor: pointer;
            width: 100%;
            transition: transform 0.2s ease;
        }
        
        .submit-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 20px rgba(102, 126, 234, 0.4);
        }
        
        .submit-btn:disabled {
            opacity: 0.6;
            cursor: not-allowed;
            transform: none;
        }
        
        .help-text {
            font-size: 13px;
            color: #666;
            margin-top: 5px;
            font-style: italic;
        }
        
        @media (max-width: 600px) {
            .form-content {
                padding: 30px 20px;
            }
            
            .header {
                padding: 30px 20px;
            }
            
            .header h1 {
                font-size: 26px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>Business Insurance Quote Request</h1>
            <p>Complete this form to receive a customized quote. A sales agent will follow up within 1-2 business days.</p>
            <p style="margin-top: 10px; font-size: 14px;">📎 Have insurance documents? You can upload them below!</p>
        </div>
        
        <div class="form-content">
            <form action="https://formspree.io/f/xgvnlkor" method="POST" enctype="multipart/form-data">
                <!-- Business Information Section -->
                <div class="section">
                    <h2 class="section-title">Business Information</h2>
                    
                    <div class="form-group">
                        <label>Business Name <span class="required">*</span></label>
                        <input type="text" name="businessName" required>
                    </div>
                    
                    <div class="form-group">
                        <label>DBA (if applicable)</label>
                        <input type="text" name="dba">
                    </div>
                    
                    <div class="form-group">
                        <label>Business Address <span class="required">*</span></label>
                        <input type="text" name="businessAddress" required>
                    </div>
                    
                    <div class="form-group">
                        <label>City <span class="required">*</span></label>
                        <input type="text" name="city" required>
                    </div>
                    
                    <div class="form-group">
                        <label>State <span class="required">*</span></label>
                        <select name="state" required>
                            <option value="">Select State</option>
                            <option value="AL">Alabama</option>
                            <option value="AK">Alaska</option>
                            <option value="AZ">Arizona</option>
                            <option value="AR">Arkansas</option>
                            <option value="CA">California</option>
                            <option value="CO">Colorado</option>
                            <option value="CT">Connecticut</option>
                            <option value="DE">Delaware</option>
                            <option value="FL">Florida</option>
                            <option value="GA">Georgia</option>
                            <option value="HI">Hawaii</option>
                            <option value="ID">Idaho</option>
                            <option value="IL">Illinois</option>
                            <option value="IN">Indiana</option>
                            <option value="IA">Iowa</option>
                            <option value="KS">Kansas</option>
                            <option value="KY">Kentucky</option>
                            <option value="LA">Louisiana</option>
                            <option value="ME">Maine</option>
                            <option value="MD">Maryland</option>
                            <option value="MA">Massachusetts</option>
                            <option value="MI">Michigan</option>
                            <option value="MN">Minnesota</option>
                            <option value="MS">Mississippi</option>
                            <option value="MO">Missouri</option>
                            <option value="MT">Montana</option>
                            <option value="NE">Nebraska</option>
                            <option value="NV">Nevada</option>
                            <option value="NH">New Hampshire</option>
                            <option value="NJ">New Jersey</option>
                            <option value="NM">New Mexico</option>
                            <option value="NY">New York</option>
                            <option value="NC">North Carolina</option>
                            <option value="ND">North Dakota</option>
                            <option value="OH">Ohio</option>
                            <option value="OK">Oklahoma</option>
                            <option value="OR">Oregon</option>
                            <option value="PA">Pennsylvania</option>
                            <option value="RI">Rhode Island</option>
                            <option value="SC">South Carolina</option>
                            <option value="SD">South Dakota</option>
                            <option value="TN">Tennessee</option>
                            <option value="TX">Texas</option>
                            <option value="UT">Utah</option>
                            <option value="VT">Vermont</option>
                            <option value="VA">Virginia</option>
                            <option value="WA">Washington</option>
                            <option value="WV">West Virginia</option>
                            <option value="WI">Wisconsin</option>
                            <option value="WY">Wyoming</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label>ZIP Code <span class="required">*</span></label>
                        <input type="text" name="zip" required>
                    </div>
                    
                    <div class="form-group">
                        <label>Business Phone <span class="required">*</span></label>
                        <input type="tel" name="businessPhone" required>
                    </div>
                    
                    <div class="form-group">
                        <label>Business Email <span class="required">*</span></label>
                        <input type="email" name="businessEmail" required>
                    </div>
                    
                    <div class="form-group">
                        <label>Website (if applicable)</label>
                        <input type="text" name="website">
                    </div>
                    
                    <div class="form-group">
                        <label>FEIN or SSN / TAX ID <span class="required">*</span></label>
                        <input type="text" name="taxId" required>
                    </div>
                    
                    <div class="form-group">
                        <label>Business Type <span class="required">*</span></label>
                        <select name="businessType" required>
                            <option value="">Select Business Type</option>
                            <option value="LLC">LLC</option>
                            <option value="S-Corp">S-Corp</option>
                            <option value="C-Corp">C-Corp</option>
                            <option value="Sole Proprietor">Sole Proprietor</option>
                            <option value="Partnership">Partnership</option>
                            <option value="Non-Profit">Non-Profit</option>
                            <option value="Other">Other</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label>Years in Business <span class="required">*</span></label>
                        <input type="number" name="yearsInBusiness" min="0" required>
                    </div>
                    
                    <div class="form-group">
                        <label>Number of Employees <span class="required">*</span></label>
                        <input type="number" name="numEmployees" min="0" required>
                    </div>
                    
                    <div class="form-group">
                        <label>Annual Payroll <span class="required">*</span></label>
                        <input type="text" name="annualPayroll" required placeholder="e.g., $250,000">
                    </div>
                    
                    <div class="form-group">
                        <label>Annual Revenue <span class="required">*</span></label>
                        <input type="text" name="annualRevenue" required placeholder="e.g., $500,000">
                    </div>
                </div>
                
                <!-- Owner Information Section -->
                <div class="section">
                    <h2 class="section-title">Owner Information</h2>
                    
                    <div class="form-group">
                        <label>Owner's Full Name <span class="required">*</span></label>
                        <input type="text" name="ownerName" required>
                    </div>
                    
                    <div class="form-group">
                        <label>Date of Birth <span class="required">*</span></label>
                        <input type="date" name="ownerDob" required>
                    </div>
                    
                    <div class="form-group">
                        <label>Phone Number <span class="required">*</span></label>
                        <input type="tel" name="ownerPhone" required>
                    </div>
                    
                    <div class="form-group">
                        <label>Email Address <span class="required">*</span></label>
                        <input type="email" name="ownerEmail" required>
                    </div>
                </div>
                
                <!-- Coverage Details Section -->
                <div class="section">
                    <h2 class="section-title">Coverage Details</h2>
                    
                    <div class="form-group">
                        <label>Type of Insurance Needed <span class="required">*</span></label>
                        <div class="checkbox-group">
                            <div class="checkbox-item">
                                <input type="checkbox" name="insuranceType" value="General Liability" id="gl">
                                <label for="gl" style="margin: 0; font-weight: normal;">General Liability</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" name="insuranceType" value="Workers Comp" id="wc">
                                <label for="wc" style="margin: 0; font-weight: normal;">Workers' Comp</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" name="insuranceType" value="BOP" id="bop">
                                <label for="bop" style="margin: 0; font-weight: normal;">BOP (Business Owner's Policy)</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" name="insuranceType" value="Commercial Auto" id="auto">
                                <label for="auto" style="margin: 0; font-weight: normal;">Commercial Auto</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" name="insuranceType" value="Professional Liability" id="pl">
                                <label for="pl" style="margin: 0; font-weight: normal;">Professional Liability (E&O)</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" name="insuranceType" value="Cyber Liability" id="cyber">
                                <label for="cyber" style="margin: 0; font-weight: normal;">Cyber Liability</label>
                            </div>
                            <div class="checkbox-item">
                                <input type="checkbox" name="insuranceType" value="Other" id="other">
                                <label for="other" style="margin: 0; font-weight: normal;">Other</label>
                            </div>
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label>Current Insurance Provider (if applicable)</label>
                        <input type="text" name="currentProvider">
                    </div>
                    
                    <div class="form-group">
                        <label>Policy Expiration Date (if applicable)</label>
                        <input type="date" name="expirationDate">
                    </div>
                    
                    <div class="form-group">
                        <label>Desired Coverage Limits</label>
                        <textarea name="coverageLimits" placeholder="e.g., $1,000,000 per occurrence / $2,000,000 aggregate"></textarea>
                    </div>
                    
                    <div class="form-group">
                        <label>Any Claims in the Last 5 Years? <span class="required">*</span></label>
                        <div class="radio-group">
                            <div class="radio-item">
                                <input type="radio" name="hasClaims" value="Yes" id="claimsYes" required>
                                <label for="claimsYes" style="margin: 0; font-weight: normal;">Yes</label>
                            </div>
                            <div class="radio-item">
                                <input type="radio" name="hasClaims" value="No" id="claimsNo">
                                <label for="claimsNo" style="margin: 0; font-weight: normal;">No</label>
                            </div>
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label>If Yes, provide claim details</label>
                        <textarea name="claimDetails" placeholder="Describe the nature of claims, dates, and amounts"></textarea>
                    </div>
                </div>
                
                <!-- Business Operations Section -->
                <div class="section">
                    <h2 class="section-title">Business Operations</h2>
                    
                    <div class="form-group">
                        <label>Industry/Business Type <span class="required">*</span></label>
                        <input type="text" name="industry" required placeholder="e.g., Construction, Restaurant, Retail">
                    </div>
                    
                    <div class="form-group">
                        <label>Describe Business Operations <span class="required">*</span></label>
                        <textarea name="businessDescription" required placeholder="Provide a detailed description of what your business does"></textarea>
                    </div>
                    
                    <div class="form-group">
                        <label>Primary Business Location <span class="required">*</span></label>
                        <select name="businessLocation" required>
                            <option value="">Select Location Type</option>
                            <option value="Office">Office</option>
                            <option value="Retail">Retail</option>
                            <option value="Home-Based">Home-Based</option>
                            <option value="Warehouse">Warehouse</option>
                            <option value="Manufacturing">Manufacturing Facility</option>
                            <option value="Multiple">Multiple Locations</option>
                            <option value="Other">Other</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label>Do Customers Visit the Premises? <span class="required">*</span></label>
                        <div class="radio-group">
                            <div class="radio-item">
                                <input type="radio" name="customersVisit" value="Yes" id="visitYes" required>
                                <label for="visitYes" style="margin: 0; font-weight: normal;">Yes</label>
                            </div>
                            <div class="radio-item">
                                <input type="radio" name="customersVisit" value="No" id="visitNo">
                                <label for="visitNo" style="margin: 0; font-weight: normal;">No</label>
                            </div>
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label>Any Business-Owned Vehicles? <span class="required">*</span></label>
                        <div class="radio-group">
                            <div class="radio-item">
                                <input type="radio" name="hasVehicles" value="Yes" id="vehiclesYes" required>
                                <label for="vehiclesYes" style="margin: 0; font-weight: normal;">Yes</label>
                            </div>
                            <div class="radio-item">
                                <input type="radio" name="hasVehicles" value="No" id="vehiclesNo">
                                <label for="vehiclesNo" style="margin: 0; font-weight: normal;">No</label>
                            </div>
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label>If Yes, provide vehicle details (Year, Make, Model, VIN)</label>
                        <textarea name="vehicleDetails" placeholder="List each vehicle with Year, Make, Model, and VIN"></textarea>
                    </div>
                    
                    <div class="form-group">
                        <label>If vehicles, provide driver information (Name, Address, DOB, DL#)</label>
                        <textarea name="driverDetails" placeholder="List each driver with Name, Address, Date of Birth, and Driver's License Number"></textarea>
                    </div>
                </div>
                
                <!-- Additional Information Section -->
                <div class="section">
                    <h2 class="section-title">Additional Information</h2>
                    
                    <div class="form-group">
                        <label>Upload Declaration Pages / Insurance Documents</label>
                        <input type="file" name="upload" accept=".pdf,.jpg,.jpeg,.png,.doc,.docx" multiple>
                        <p class="help-text">Upload current declaration pages, loss history report, or other relevant insurance documents (PDF, JPG, PNG, DOC - Max 10MB total)</p>
                    </div>
                    
                    <div class="form-group">
                        <label>Additional Notes or Special Requests</label>
                        <textarea name="additionalNotes" placeholder="Any other coverage needs, endorsements, or special considerations"></textarea>
                    </div>
                    
                    <div class="form-group">
                        <label>How did you hear about us?</label>
                        <select name="referralSource">
                            <option value="">Select...</option>
                            <option value="Google Search">Google Search</option>
                            <option value="Referral">Referral</option>
                            <option value="Social Media">Social Media</option>
                            <option value="Advertisement">Advertisement</option>
                            <option value="Existing Client">Existing Client</option>
                            <option value="Other">Other</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label>Preferred Contact Method <span class="required">*</span></label>
                        <div class="radio-group">
                            <div class="radio-item">
                                <input type="radio" name="contactMethod" value="Phone" id="contactPhone" required>
                                <label for="contactPhone" style="margin: 0; font-weight: normal;">Phone</label>
                            </div>
                            <div class="radio-item">
                                <input type="radio" name="contactMethod" value="Email" id="contactEmail">
                                <label for="contactEmail" style="margin: 0; font-weight: normal;">Email</label>
                            </div>
                            <div class="radio-item">
                                <input type="radio" name="contactMethod" value="Either" id="contactEither">
                                <label for="contactEither" style="margin: 0; font-weight: normal;">Either</label>
                            </div>
                        </div>
                    </div>
                </div>
                
                <button type="submit" class="submit-btn">Submit Quote Request</button>
            </form>
        </div>
    </div>
</body>
</html>

